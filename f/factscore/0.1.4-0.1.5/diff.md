# Comparing `tmp/factscore-0.1.4.tar.gz` & `tmp/factscore-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factscore-0.1.4.tar", max compression
+gzip compressed data, was "factscore-0.1.5.tar", max compression
```

## Comparing `factscore-0.1.4.tar` & `factscore-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4162 2023-05-23 23:32:42.536727 factscore-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.4/factscore/__init__.py
--rw-r--r--   0        0        0    15249 2023-05-23 19:22:54.093599 factscore-0.1.4/factscore/atomic_facts.py
--rw-r--r--   0        0        0     2967 2023-05-23 14:51:37.783672 factscore-0.1.4/factscore/clm.py
--rw-r--r--   0        0        0     2360 2023-05-23 20:34:54.535604 factscore-0.1.4/factscore/download_data.py
--rw-r--r--   0        0        0    10241 2023-05-23 19:39:46.119599 factscore-0.1.4/factscore/factscorer.py
--rw-r--r--   0        0        0     1706 2023-05-23 19:09:54.010548 factscore-0.1.4/factscore/lm.py
--rw-r--r--   0        0        0     7105 2023-05-23 19:37:35.506439 factscore-0.1.4/factscore/npm.py
--rw-r--r--   0        0        0     3956 2023-05-23 19:20:40.884494 factscore-0.1.4/factscore/openai_lm.py
--rw-r--r--   0        0        0     7747 2023-05-23 19:31:41.778130 factscore-0.1.4/factscore/retrieval.py
--rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.4/factscore/utils.py
--rw-r--r--   0        0        0      813 2023-05-23 23:33:14.440003 factscore-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 factscore-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     9346 2023-06-06 17:21:42.894924 factscore-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.5/factscore/__init__.py
+-rw-r--r--   0        0        0    16060 2023-06-06 15:53:00.787244 factscore-0.1.5/factscore/atomic_facts.py
+-rw-r--r--   0        0        0     2868 2023-05-26 23:16:58.269806 factscore-0.1.5/factscore/clm.py
+-rw-r--r--   0        0        0     6178 2023-05-26 23:16:58.269806 factscore-0.1.5/factscore/download_data.py
+-rw-r--r--   0        0        0    14229 2023-06-06 15:53:00.787244 factscore-0.1.5/factscore/factscorer.py
+-rw-r--r--   0        0        0     1691 2023-05-26 23:16:58.269806 factscore-0.1.5/factscore/lm.py
+-rw-r--r--   0        0        0     7105 2023-05-23 19:37:35.506439 factscore-0.1.5/factscore/npm.py
+-rw-r--r--   0        0        0     4090 2023-05-26 23:16:58.269806 factscore-0.1.5/factscore/openai_lm.py
+-rw-r--r--   0        0        0     7747 2023-05-23 19:31:41.778130 factscore-0.1.5/factscore/retrieval.py
+-rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.5/factscore/utils.py
+-rw-r--r--   0        0        0      813 2023-06-06 17:18:08.031618 factscore-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    10467 1970-01-01 00:00:00.000000 factscore-0.1.5/PKG-INFO
```

### Comparing `factscore-0.1.4/factscore/atomic_facts.py` & `factscore-0.1.5/factscore/atomic_facts.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,25 +34,27 @@
         # get the demos
         with open(self.demon_path, 'r') as f:
             self.demons = json.load(f)
 
         tokenized_corpus = [doc.split(" ") for doc in self.demons.keys()]
         self.bm25 = BM25Okapi(tokenized_corpus)
 
-    def run(self, generation):
-        """Convert the generation into a set of atomic facts."""
+    def save_cache(self):
+        self.openai_lm.save_cache()
+
+    def run(self, generation, cost_estimate=None):
+        """Convert the generation into a set of atomic facts. Return a total words cost if cost_estimate != None."""
         if self.preprocess_fn:
             paragraphs = self.preprocess(generation)
         else:
             paragraphs = [para.strip() for para in generation.split("\n") if len(para.strip()) > 0]
 
-        atomic_facts, para_breaks = self.get_atomic_facts_from_paragraph(paragraphs)
-        return atomic_facts, para_breaks
+        return self.get_atomic_facts_from_paragraph(paragraphs, cost_estimate=cost_estimate)
 
-    def get_atomic_facts_from_paragraph(self, paragraphs):
+    def get_atomic_facts_from_paragraph(self, paragraphs, cost_estimate=None):
         sentences = []
         para_breaks = []
         for para_idx, paragraph in enumerate(paragraphs):
             if para_idx > 0 :
                 para_breaks.append(len(sentences))
 
             initials = detect_initials(paragraph)
@@ -64,17 +66,22 @@
             curr_sentences_2 = fix_sentence_splitter(curr_sentences_2, initials)
 
             # checking this, just to ensure the crediability of the sentence splitter fixing algorithm
             assert curr_sentences == curr_sentences_2, (paragraph, curr_sentences, curr_sentences_2)
 
             sentences += curr_sentences
 
-        atoms = self.get_init_atomic_facts_from_sentence([sent for i, sent in enumerate(sentences) if not (not self.is_bio and ( \
-                    (i==0 and (sent.startswith("Sure") or sent.startswith("Here are"))) or \
-                    (i==len(sentences)-1 and (sent.startswith("Please") or sent.startswith("I hope") or sent.startswith("Here are")))))])
+        atoms_or_estimate = self.get_init_atomic_facts_from_sentence([sent for i, sent in enumerate(sentences) if not (not self.is_bio and ( \
+                            (i==0 and (sent.startswith("Sure") or sent.startswith("Here are"))) or \
+                            (i==len(sentences)-1 and (sent.startswith("Please") or sent.startswith("I hope") or sent.startswith("Here are")))))], cost_estimate=cost_estimate)
+
+        if cost_estimate:
+            return atoms_or_estimate
+        else:
+            atoms = atoms_or_estimate
 
         atomic_facts_pairs = []
         for i, sent in enumerate(sentences):
             if not self.is_bio and ( \
                 (i==0 and (sent.startswith("Sure") or sent.startswith("Here are"))) or \
                 (i==len(sentences)-1 and (sent.startswith("Please") or sent.startswith("I hope") or sent.startswith("Here are")))):
                 atomic_facts_pairs.append((sent, []))
@@ -91,15 +98,17 @@
         # the new para_breaks should be identical to the original para_breaks
         if self.is_bio:
             atomic_facts_pairs, para_breaks = postprocess_atomic_facts(atomic_facts_pairs, list(para_breaks), self.nlp)
 
         return atomic_facts_pairs, para_breaks
 
 
-    def get_init_atomic_facts_from_sentence(self, sentences):
+    def get_init_atomic_facts_from_sentence(self, sentences, cost_estimate=None):
+        """Get the initial atomic facts from the sentences. Return a total words cost if cost_estimate != None."""
+
         is_bio = self.is_bio
         demons = self.demons
 
         k = 1 if is_bio else 0
         n = 7 if is_bio else 8
 
         prompts = []
@@ -122,23 +131,31 @@
                 for fact in demons[match]:
                     prompt = prompt + "- {}\n".format(fact)
                 prompt = prompt + "\n"
             prompt = prompt + "Please breakdown the following sentence into independent facts: {}\n".format(sentence)
             prompts.append(prompt)
             prompt_to_sent[prompt] = sentence
 
-        for prompt in prompts:
-            output, _ = self.openai_lm.generate(prompt)
-            atoms[prompt_to_sent[prompt]] = text_to_sentences(output)
-
-        for key, value in demons.items():
-            if key not in atoms:
-                atoms[key] = value
+        if cost_estimate:
+            total_words_estimate = 0
+            for prompt in prompts:
+                if cost_estimate == "consider_cache" and (prompt.strip() + "_0") in self.openai_lm.cache_dict:
+                    continue
+                total_words_estimate += len(prompt.split())
+            return total_words_estimate
+        else:
+            for prompt in prompts:
+                output, _ = self.openai_lm.generate(prompt)
+                atoms[prompt_to_sent[prompt]] = text_to_sentences(output)
+
+            for key, value in demons.items():
+                if key not in atoms:
+                    atoms[key] = value
 
-        return atoms
+            return atoms
 
 
 def preprocess_fn(generation, model):
     if model in ["instruct", "gpt4", "vicuna-7b", "vicuna-13b", "chatgpt"]:
         if not generation.startswith("I'm sorry") and not "provide more" in generation:
             paragraphs = [para.strip() for para in generation.split("\n") if len(para.strip()) > 0]
         else:
```

### Comparing `factscore-0.1.4/factscore/clm.py` & `factscore-0.1.5/factscore/clm.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         if verbose:
             input_ids = tqdm(input_ids)
 
         generations = []
         scores = []
         for curr_input_ids in input_ids:
             if len(curr_input_ids) > max_sequence_length - max_output_length:
-                print("length exceeded {} ({})!".format(max_sequence_length, len(curr_input_ids)))
                 curr_input_ids = curr_input_ids[-(max_sequence_length - max_output_length):]
             curr_input_ids = torch.LongTensor([curr_input_ids]).cuda()
             gen_outputs = self.model.generate(
                 curr_input_ids,
                 max_length=curr_input_ids.shape[1]+max_output_length,
                 return_dict_in_generate=True,
                 output_scores=True
```

### Comparing `factscore-0.1.4/factscore/factscorer.py` & `factscore-0.1.5/factscore/factscorer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 import argparse
 import string
 import json
 import numpy as np
 import os
+import logging
 
 from tqdm import tqdm
 from factscore.atomic_facts import AtomicFactGenerator
 from factscore.clm import CLM
 from factscore.npm import NPM
 from factscore.openai_lm import OpenAIModel
 from factscore.retrieval import DocDB, Retrieval
 
 class FactScorer(object):
 
     def __init__(self,
                  model_name="retrieval+ChatGPT",
+                 data_dir=".cache/factscore",
+                 model_dir=".cache/factscore",
                  cache_dir=".cache/factscore",
                  openai_key="api.key",
+                 cost_estimate="consider_cache",
                  batch_size=256):
         assert model_name in ["retrieval+llama", "retrieval+llama+npm", "retrieval+ChatGPT", "npm", "retrieval+ChatGPT+npm"]
         self.model_name = model_name
 
         self.db = {}
         self.retrieval = {}
         self.npm = {}
         self.batch_size = batch_size # batch size for retrieval
         self.openai_key = openai_key
 
+        self.data_dir = data_dir
         self.cache_dir = cache_dir
         if not os.path.exists(cache_dir):
             os.makedirs(cache_dir)
 
         self.af_generator = None
+        self.cost_estimate = cost_estimate
 
         if "llama" in model_name:
             self.lm = CLM("inst-llama-7B",
-                          model_dir=os.path.join(cache_dir, "inst-llama-7B"),
+                          model_dir=os.path.join(model_dir, "inst-llama-7B"),
                           cache_file=os.path.join(cache_dir, "inst-llama-7B.pkl"))
         elif "ChatGPT" in model_name:
             self.lm = OpenAIModel("ChatGPT",
                                   cache_file=os.path.join(cache_dir, "ChatGPT.pkl"),
                                   key_path=openai_key)
         else:
             self.lm = None
@@ -52,44 +58,62 @@
                 v.save_cache()
         for k, v in self.retrieval.items():
             v.save_cache()
 
     def register_knowledge_source(self, name="enwiki-20230401", db_path=None, data_path=None):
         assert name not in self.retrieval, f"{name} already registered"
         if db_path is None:
-            db_path = os.path.join(self.cache_dir, f"{name}.db")
+            db_path = os.path.join(self.data_dir, f"{name}.db")
 
         if data_path is None:
-            data_path = os.path.join(self.cache_dir, f"{name}.jsonl")
+            data_path = os.path.join(self.data_dir, f"{name}.jsonl")
 
         cache_path = os.path.join(self.cache_dir, f"retrieval-{name}.json")
         embed_cache_path = os.path.join(self.cache_dir, f"retrieval-{name}.pkl")
 
         self.db[name] = DocDB(db_path=db_path, data_path=data_path)
         self.retrieval[name] = Retrieval(self.db[name], cache_path, embed_cache_path, batch_size=self.batch_size)
         if "npm" in self.model_name:
             cache_path = os.path.join(self.cache_dir, f"bm25-{name}.json")
             embed_cache_path = os.path.join(self.cache_dir, f"bm25-{name}.pkl")
             self.npm[name] = NPM(Retrieval(self.db[name], cache_path, embed_cache_path, "bm25"),
                                  "npm-single",
                                  cache_file=os.path.join(self.cache_dir, f"npm-{name}.pkl"))
 
+
+    def print_cost_estimates(self, total_words, task, model):
+        # https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them
+        # Number of tokens are roughly 4/3 of the number of words
+        total_tokens = total_words * 4.0 / 3
+
+        # https://openai.com/pricing
+        # if we use davinci-003, the cost is $0.02 per 1000 tokens
+        # if we use gpt-3.5-turbo, the cost is $0.002 per 1000 tokens
+        if model == "davinci-003":
+            rate = 0.02
+        elif model == "gpt-3.5-turbo":
+            rate = 0.002
+
+        total_cost = total_tokens * rate / 1000
+
+        # print the total words, tokens, and cost along with rate
+        logging.critical("Estimated OpenAI API cost for %s ($%.3f per 1000 tokens): $%.2f for %d words and %d tokens" % (task, rate, total_cost, total_words, total_tokens))
+
     def get_score(self,
                   topics,
                   generations,
                   atomic_facts=None,
                   knowledge_source=None,
-                  return_atomic_facts=False,
-                  return_individual_decisions=False,
                   verbose=False):
 
         if knowledge_source is None:
             # use the default one (enwiki-20230401)
             knowledge_source = "enwiki-20230401"
-            self.register_knowledge_source(knowledge_source)
+            if knowledge_source not in self.retrieval:
+                self.register_knowledge_source(knowledge_source)
         else:
             assert knowledge_source in self.retrieval, \
                 f"{knowledge_source} is not registered yet. Please use `register_knowledge_source()` function to register it with a database"
 
         if type(topics)==len(generations)==str:
             topics = [topics]
             generations = [generations]
@@ -98,65 +122,98 @@
             assert len(topics)==len(generations), "`topics` and `generations` should have the same length"
 
         if atomic_facts is not None:
             assert len(topics)==len(atomic_facts), "`topics` and `atomic_facts` should have the same length"
         else:
             if self.af_generator is None:
                 self.af_generator = AtomicFactGenerator(key_path=self.openai_key,
-                                                        demon_dir=os.path.join(self.cache_dir, "demos"),
+                                                        demon_dir=os.path.join(self.data_dir, "demos"),
                                                         gpt3_cache_file=os.path.join(self.cache_dir, "InstructGPT.pkl"))
 
+            # estimate the total cost of atomic fact generation
+            total_words = 0
+            for gen in generations:
+                total_words += self.af_generator.run(gen, cost_estimate=self.cost_estimate)
+
+            self.print_cost_estimates(total_words, task="atomic fact generation", model="davinci-003")
+
             if verbose:
                 topics = tqdm(topics)
 
-            new_topics, new_generations, new_atomic_facts = [], [], []
+            atomic_facts = []
             for topic, gen in zip(topics, generations):
                 curr_afs, _ = self.af_generator.run(gen)
                 curr_afs = [fact for _, facts in curr_afs for fact in facts]
                 if len(curr_afs)==0:
-                    # abstain from answering
-                    continue
-                new_topics.append(topic)
-                new_generations.append(gen)
-                new_atomic_facts.append(curr_afs)
-            topics, generations, atomic_facts = new_topics, new_generations, new_atomic_facts
+                    atomic_facts.append(None)
+                else:
+                    atomic_facts.append(curr_afs)
+                if len(atomic_facts) % 10 == 0:
+                    self.af_generator.save_cache()
+
+            assert len(atomic_facts)==len(topics)
+            self.af_generator.save_cache()
+
+        respond_ratio = np.mean([facts is not None for facts in atomic_facts])
+
+        if "ChatGPT" in self.model_name:
+            # estimate the total cost of response generation
+            total_words = 0
+            for topic, generation, facts in zip(topics, generations, atomic_facts):
+                if facts is not None:
+                    total_words += self._get_score(topic, generation, facts, knowledge_source, cost_estimate=self.cost_estimate)
+
+            self.print_cost_estimates(total_words, task="factscore evaluation", model="gpt-3.5-turbo")
 
         if verbose:
             topics = tqdm(topics)
 
         scores = []
         decisions = []
         for topic, generation, facts in zip(topics, generations, atomic_facts):
-            decision = self._get_score(topic, generation, facts, knowledge_source)
-            score = np.mean([d["is_supported"] for d in decision])
-            decisions.append(decision)
-            scores.append(score)
-
-        if return_atomic_facts:
-            return np.mean(scores), atomic_facts
-
-        if return_individual_decisions:
-            return np.mean(scores), decisions
-
-        return np.mean(scores)
+            if facts is None:
+                decisions.append(None)
+            else:
+                decision = self._get_score(topic, generation, facts, knowledge_source)
+                score = np.mean([d["is_supported"] for d in decision])
+                decisions.append(decision)
+                scores.append(score)
+                if len(scores) % 10 == 0:
+                    self.save_cache()
+
+        self.save_cache()
+
+        return {"score": np.mean(scores),
+                "respond_ratio": respond_ratio,
+                "decisions": decisions,
+                "num_facts_per_response": np.mean([len(d) for d in decisions if d is not None])}
 
-    def _get_score(self, topic, generation, atomic_facts, knowledge_source):
+    def _get_score(self, topic, generation, atomic_facts, knowledge_source, cost_estimate=None):
         decisions = []
+        total_words = 0
         for atom in atomic_facts:
             atom = atom.strip()
             if self.lm:
                 passages = self.retrieval[knowledge_source].get_passages(topic, atom, k=5)
                 definition = "Answer the question about {} based on the given context.\n\n".format(topic)
                 context = ""
                 for psg_idx, psg in enumerate(reversed(passages)):
                     context += "Title: {}\nText: {}\n\n".format(psg["title"], psg["text"].replace("<s>", "").replace("</s>", ""))
                 definition += context.strip()
                 if not definition[-1] in string.punctuation:
                     definition += "."
                 prompt = "{}\n\nInput: {} True or False?\nOutput:".format(definition.strip(), atom.strip())
+
+                if cost_estimate:
+                    if cost_estimate == "consider_cache" and (prompt.strip() + "_0") not in self.lm.cache_dict:
+                        total_words += len(prompt.split())
+                    elif cost_estimate == "ignore_cache":
+                        total_words += len(prompt.split())
+                    continue
+
                 output = self.lm.generate(prompt)
 
                 if type(output[1])==np.ndarray:
                     # when logits are available
                     logits = np.array(output[1])
                     assert logits.shape[0] in [32000, 32001]
                     true_score = logits[5852]
@@ -178,49 +235,74 @@
             else:
                 is_supported = True
 
             if is_supported and "npm" in self.model_name:
                 npprob = self.npm[knowledge_source].get_probabilty(topic, atom)
                 is_supported = npprob > 0.3
 
-            decisions.append({"atom": atom,
-                              "is_supported": is_supported})
+            decisions.append({"atom": atom, "is_supported": is_supported})
 
-        return decisions
+        if cost_estimate:
+            return total_words
+        else:
+            return decisions
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('--data_path',
+    parser.add_argument('--input_path',
                         type=str,
                         default="data/labeled/InstructGPT.jsonl")
     parser.add_argument('--model_name',
                         type=str,
                         default="retrieval+ChatGPT")
     parser.add_argument('--openai_key',
                         type=str,
                         default="api.key")
+    parser.add_argument('--data_dir',
+                        type=str,
+                        default=".cache/factscore/")
+    parser.add_argument('--model_dir',
+                        type=str,
+                        default=".cache/factscore/")
     parser.add_argument('--cache_dir',
                         type=str,
                         default=".cache/factscore/")
+    parser.add_argument('--cost_estimate',
+                        type=str,
+                        default="consider_cache",
+                        choices=["consider_cache", "ignore_cache"])
     parser.add_argument('--use_atomic_facts',
                         action="store_true")
     parser.add_argument('--verbose',
-                        action="store_true")
+                        action="store_true",
+                        help="for printing out the progress bar")
+    parser.add_argument('--print_rate_limit_error',
+                        action="store_true",
+                        help="for printing out rate limit error when using OpenAI keys")
     parser.add_argument('--n_samples',
                         type=int,
                         default=None)
 
     args = parser.parse_args()
 
-    fs = FactScorer(args.model_name, args.cache_dir, args.openai_key)
+    logging.basicConfig(format='%(asctime)s - %(name)s - %(message)s',
+                        datefmt='%m/%d/%Y %H:%M:%S',
+                        level=logging.ERROR if args.print_rate_limit_error else logging.CRITICAL)
+
+    fs = FactScorer(model_name=args.model_name,
+                    data_dir=args.data_dir,
+                    model_dir=args.model_dir,
+                    cache_dir=args.cache_dir,
+                    openai_key=args.openai_key,
+                    cost_estimate=args.cost_estimate)
 
     tot = 0
     topics, generations, atomic_facts = [], [], []
-    with open(args.data_path) as f:
+    with open(args.input_path) as f:
         for line in f:
             dp = json.loads(line)
             tot += 1
             if args.use_atomic_facts:
                 assert "annotations" in dp, "You can specify `--use_atomic_facts` only when atomic facts are available in the input data already."
                 if dp["annotations"] is None:
                     continue
@@ -228,14 +310,17 @@
                 generations.append(dp["output"])
                 atomic_facts.append([atom["text"] for sent in dp["annotations"] for atom in sent["model-atomic-facts"]])
             else:
                 topics.append(dp["topic"])
                 generations.append(dp["output"])
             if args.n_samples is not None and tot==args.n_samples:
                 break
-
-    score = fs.get_score(topics=topics, generations=generations, atomic_facts=atomic_facts if args.use_atomic_facts else None, verbose=args.verbose)
-    print (score)
-    fs.save_cache()
+    out = fs.get_score(topics=topics,
+                       generations=generations,
+                       atomic_facts=atomic_facts if args.use_atomic_facts else None,
+                       verbose=args.verbose)
+    logging.critical("FActScore = %.1f%%" % (100*out["score"]))
+    logging.critical("Respond ratio = %.1f%%" % (100*out["respond_ratio"]))
+    logging.critical("# Atomic facts per valid response = %.1f" % (out["num_facts_per_response"]))
```

### Comparing `factscore-0.1.4/factscore/lm.py` & `factscore-0.1.5/factscore/lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.model = None
         self.add_n = 0
 
     def load_model(self):
         # load the model and put it as self.model
         raise NotImplementedError()
 
-    def generate(self, prompt, sample_idx=0, max_sequence_length=2048, max_output_length=128, verbose=False):
+    def generate(self, prompt, sample_idx=0, max_sequence_length=2048, max_output_length=128):
         prompt = prompt.strip() # it's important not to end with a whitespace
         cache_key = f"{prompt}_{sample_idx}"
 
         if cache_key in self.cache_dict:
             return self.cache_dict[cache_key]
 
         if self.model is None:
```

### Comparing `factscore-0.1.4/factscore/npm.py` & `factscore-0.1.5/factscore/npm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.4/factscore/openai_lm.py` & `factscore-0.1.5/factscore/openai_lm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from factscore.lm import LM
 import openai
 import sys
 import time
 import os
 import numpy as np
-
-
+import logging
 
 class OpenAIModel(LM):
 
     def __init__(self, model_name, cache_file=None, key_path="api.key"):
         self.model_name = model_name
         self.key_path = key_path
         self.temp = 0.7
@@ -40,17 +39,18 @@
             return output, response
         elif self.model_name == "InstructGPT":
             # Call API
             response = call_GPT3(prompt, temp=self.temp)
             # Get the output from the response
             output = response["choices"][0]["text"]
             return output, response
+        else:
+            raise NotImplementedError()
 
-
-def call_ChatGPT(message, model_name="gpt-3.5-turbo", max_len=1024, temp=0.7):
+def call_ChatGPT(message, model_name="gpt-3.5-turbo", max_len=1024, temp=0.7, verbose=False):
     # call GPT-3 API until result is provided and then return it
     response = None
     received = False
     num_rate_errors = 0
     while not received:
         try:
             response = openai.ChatCompletion.create(model=model_name,
@@ -60,23 +60,23 @@
             received = True
         except:
             # print(message)
             num_rate_errors += 1
             error = sys.exc_info()[0]
             if error == openai.error.InvalidRequestError:
                 # something is wrong: e.g. prompt too long
-                print(f"InvalidRequestError\nPrompt passed in:\n\n{message}\n\n")
+                logging.critical(f"InvalidRequestError\nPrompt passed in:\n\n{message}\n\n")
                 assert False
             
-            print("API error: %s (%d). Waiting %dsec" % (error, num_rate_errors, np.power(2, num_rate_errors)))
+            logging.error("API error: %s (%d). Waiting %dsec" % (error, num_rate_errors, np.power(2, num_rate_errors)))
             time.sleep(np.power(2, num_rate_errors))
     return response
 
 
-def call_GPT3(prompt, model_name="text-davinci-003", max_len=512, temp=0.7, num_log_probs=0, echo=False):
+def call_GPT3(prompt, model_name="text-davinci-003", max_len=512, temp=0.7, num_log_probs=0, echo=False, verbose=False):
     # call GPT-3 API until result is provided and then return it
     response = None
     received = False
     num_rate_errors = 0
     while not received:
         try:
             response = openai.Completion.create(model=model_name,
@@ -87,12 +87,12 @@
                                                 echo=echo)
             received = True
         except:
             error = sys.exc_info()[0]
             num_rate_errors += 1
             if error == openai.error.InvalidRequestError:
                 # something is wrong: e.g. prompt too long
-                print(f"InvalidRequestError\nPrompt passed in:\n\n{prompt}\n\n")
+                logging.critical(f"InvalidRequestError\nPrompt passed in:\n\n{prompt}\n\n")
                 assert False
-            print("API error: %s (%d)" % (error, num_rate_errors))
+            logging.error("API error: %s (%d)" % (error, num_rate_errors))
             time.sleep(np.power(2, num_rate_errors))
     return response
```

### Comparing `factscore-0.1.4/factscore/retrieval.py` & `factscore-0.1.5/factscore/retrieval.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.4/factscore/utils.py` & `factscore-0.1.5/factscore/utils.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.4/pyproject.toml` & `factscore-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "factscore"
-version = "0.1.4"
+version = "0.1.5"
 description = "FactScore is an automatic evaluation metric for factual precision in long-form text generation. It uses large language models and retrieval to break down generations into atomic facts and then measure the correctness with respect to a knowledge source (like Wikipedia)."
 authors = ["Sewon Min <sewon@cs.washington.edu>", "Kalpesh Krishna <kalpesh@cs.umass.edu>", "Xinxi Lyu <alrope@cs.washington.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
```

