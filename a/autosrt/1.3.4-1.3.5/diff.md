# Comparing `tmp/autosrt-1.3.4.tar.gz` & `tmp/autosrt-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.4.tar", last modified: Mon Jun  5 01:31:00 2023, max compression
+gzip compressed data, was "autosrt-1.3.5.tar", last modified: Tue Jun  6 21:19:03 2023, max compression
```

## Comparing `autosrt-1.3.4.tar` & `autosrt-1.3.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.878979 autosrt-1.3.4/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-05 01:31:00.878979 autosrt-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.837025 autosrt-1.3.4/autosrt/
--rw-rw-rw-   0        0        0    16163 2023-06-05 01:30:32.000000 autosrt-1.3.4/autosrt/__init__.py
--rw-rw-rw-   0        0        0    71573 2023-06-05 01:26:11.000000 autosrt-1.3.4/autosrt/autosrt.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.858751 autosrt-1.3.4/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-05 01:31:00.883475 autosrt-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.875983 autosrt-1.3.4/test/
--rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.4/test/test1.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.4/test/test2.py
--rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.4/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.4/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.197996 autosrt-1.3.5/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-06 21:19:03.198746 autosrt-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.161617 autosrt-1.3.5/autosrt/
+-rw-rw-rw-   0        0        0   116952 2023-06-06 21:18:37.000000 autosrt-1.3.5/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.186008 autosrt-1.3.5/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-06 21:19:03.000000 autosrt-1.3.5/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 21:19:02.000000 autosrt-1.3.5/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-06 21:19:03.201744 autosrt-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:19:03.196498 autosrt-1.3.5/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.3.5/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.3.5/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.3.5/test/test3.py
+-rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.5/test/test4.py
```

### Comparing `autosrt-1.3.4/LICENSE` & `autosrt-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.4/PKG-INFO` & `autosrt-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.4
+Version: 1.3.5
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.4/README.md` & `autosrt-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.4/autosrt/__init__.py` & `autosrt-1.3.5/test/test3.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,72 @@
 from __future__ import absolute_import, print_function, unicode_literals
 import argparse
 import os
 import sys
 import multiprocessing
-from glob import glob, escape
+from glob import glob
 from progressbar import ProgressBar, Percentage, Bar, ETA
-import time
-from datetime import datetime, timedelta
-from pathlib import Path
-import subprocess
-
-from .autosrt import VERSION, Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
-    SubtitleFormatter,  SubtitleWriter, MediaSubtitleRenderer, stop_ffmpeg_windows, stop_ffmpeg_linux, remove_temp_files, \
-    is_same_language, check_file_type
-
-def has_subtitles(media_filepath):
-    if "\\" in media_filepath:
-        media_filepath = media_filepath.replace("\\", "/")
-
-    ffmpeg_cmd = [
-        "ffmpeg",
-        "-y",
-        "-i", media_filepath,
-        "-map", "0:s:0",
-        "-f", "srt",
-        "-"
-    ]
-
-    result = subprocess.run(ffmpeg_cmd, capture_output=True, text=True)
-    #print(result.stdout)
-    #print(result.stderr)
 
-    if result.stdout:
-        return True  # Subtitles detected
-    else:
-        return False  # No subtitles detected
+from autosrt import VERSION, Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
+    SubtitleFormatter,  SubtitleWriter, MediaSubtitleEmbedder, stop_ffmpeg_windows, stop_ffmpeg_linux, remove_temp_files, \
+    is_same_language, check_file_type, has_subtitles
 
 def show_progress(media_filepath, progress):
     global pbar
+    print("media_filepath = {}".format(media_filepath))
     pbar.update(progress)
 
 def show_error_messages(messages):
     print(messages)
 
 def main():
-    global pbar
+    global pbar, media_filepath
 
     if sys.platform == "win32":
         stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
     remove_temp_files("flac", error_messages_callback=show_error_messages)
     remove_temp_files("wav", error_messages_callback=show_error_messages)
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('source_path', help="Path to the video or audio files to generate subtitles files (use wildcard for multiple files or separate them with a space character e.g. \"file 1.mp4\" \"file 2.mp4\")", nargs='*')
+    parser.add_argument('source_path', help="File path of the video or audio files to generate subtitles files (use wildcard for multiple files or separate them with a space character)", nargs='*')
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-ll', '--list-languages', help="List all supported languages", action='store_true')
+    parser.add_argument('-o', '--output', help="Output file path for subtitles (by default, subtitles are saved in the same directory and named with the source_path base name)")
     parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
     parser.add_argument('-lf', '--list-formats', help="List all supported subtitle formats", action='store_true')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
-    parser.add_argument('-r', '--render', help="Boolean value (True or False) for render subtitle file into video file", type=bool, default=False)
     parser.add_argument('-v', '--version', action='version', version=VERSION)
 
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
         print("List of supported languages:")
         for code, language in sorted(language.name_of_code.items()):
             #print("{code}\t{language}".format(code=code, language=language))
             #print("%8s\t%s" %(code, language))
-            print("%-8s : %s" %(code, language))
+            print("%8s : %s" %(code, language))
         return 0
 
     #if args.src_language not in language.dict:
     if args.src_language not in language.name_of_code.keys():
         print("Source language is not supported. Run with --list-languages to see all supported languages.")
         return 1
 
     if args.dst_language:
         #if not args.dst_language in language.dict:
         if not args.dst_language in language.name_of_code.keys():
             print("Destination language is not supported. Run with --list-languages to see all supported languages.")
             return 1
-        if not is_same_language(args.src_language, args.dst_language, error_messages_callback=show_error_messages):
+        if not is_same_language(args.src_language, args.dst_language):
             do_translate = True
         else:
             do_translate = False
     else:
         do_translate = False
 
     if args.list_formats:
@@ -104,121 +79,48 @@
         print("Subtitle format is not supported. Run with --list-formats to see all supported formats.")
         return 1
 
     if not args.source_path:
         parser.print_help(sys.stderr)
         return 1
 
-    if str(args.render) == "true":
-        args.render = True
-    if str(args.render) == "false":
-        args.render = False
-
-    completed_tasks = 0
     media_filepaths = []
     arg_filepaths = []
-    invalid_media_filepaths = []
-    not_exist_filepaths = []
-    argpath = None
-    media_type = None
-
-    #for arg in args.source_path:
-    #    print("escape(arg) = %s" %(escape(arg)))
-
-    args_source_path = args.source_path
-
-    if (not "*" in str(args_source_path)) and (not "?" in str(args_source_path)):
-        for filepath in args_source_path:
-            fpath = Path(filepath)
-            #print("fpath = %s" %fpath)
-            if not os.path.isfile(fpath):
-                not_exist_filepaths.append(filepath)
-                #print(str(fpath) + " is not exist")
-
-    if sys.platform == "win32":
-        for i in range(len(args.source_path)):
-            if ("[" or "]") in args.source_path[i]:
-                placeholder = "#TEMP#"
-                args_source_path[i] = args.source_path[i].replace("[", placeholder)
-                args_source_path[i] = args_source_path[i].replace("]", "[]]")
-                args_source_path[i] = args_source_path[i].replace(placeholder, "[[]")
-                #print("args_source_path = %s" %(args_source_path))
-
-    for arg in args_source_path:
-        if not sys.platform == "win32" :
-            arg = escape(arg)
-
-        #print("glob(arg) = %s" %(glob(arg)))
 
+    for arg in args.source_path:
         arg_filepaths += glob(arg)
-        #print("arg_filepaths = %s" %(arg_filepaths))
 
-
-    if arg_filepaths:
-        for argpath in arg_filepaths:
-            if os.path.isfile(argpath):
-                if check_file_type(argpath, error_messages_callback=show_error_messages) == 'video':
-                    media_filepaths.append(argpath)
-                    media_type = "video"
-                elif check_file_type(argpath, error_messages_callback=show_error_messages) == 'audio':
-                    media_filepaths.append(argpath)
-                    media_type = "audio"
-                else:
-                    invalid_media_filepaths.append(argpath)
-                    media_type = None
+    for arg in arg_filepaths:
+        if os.path.isfile(arg):
+            if is_video_file(arg) or is_audio_file(arg):
+                media_filepaths.append(arg)
             else:
-                not_exist_filepaths.append(argpath)
-                media_type = None
-
-        if invalid_media_filepaths:
-            for invalid_media_filepath in invalid_media_filepaths:
-                msg = "{} is not valid video or audio files".format(invalid_media_filepath)
-                print(msg)
-
-    #print("not_exist_filepaths = %s" %(not_exist_filepaths))
-
-    if not_exist_filepaths:
-        if (not "*" in str(args_source_path)) and (not "?" in str(args_source_path)):
-            for not_exist_filepath in not_exist_filepaths:
-                msg = "{} is not exist".format(not_exist_filepath)
-                print(msg)
-                sys.exit(0)
-
-    if not arg_filepaths and not not_exist_filepaths:
-        print("No any files matching filenames you typed")
-        sys.exit(0)
-
-    pool = multiprocessing.Pool(args.concurrency)
-
-    transcribe_end_time = None
-    transcribe_elapsed_time = None
-    transcribe_start_time = time.time()
-    rendered_media_filepath = None
+                print("{} is not a valid video or audio file".format(arg))
+        else:
+            print("{} is not exist".format(arg))
 
     for media_filepath in media_filepaths:
-        if has_subtitles(media_filepath):
-            media_filepaths.remove(media_filepath)
+        print("Processing {} :".format(media_filepath))
 
-    for media_filepath in media_filepaths:
-        print("Processing {}".format(media_filepath))
+        widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
+        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+        wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
+        wav_filepath, sample_rate = wav_converter(media_filepath)
+        pbar.finish()
 
-        try:
-            widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
-            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-            wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
-            wav_filepath, sample_rate = wav_converter(media_filepath)
-            pbar.finish()
+        region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
+        regions = region_finder(wav_filepath)
 
-            region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
-            regions = region_finder(wav_filepath)
+        converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
+        recognizer = SpeechRecognizer(language=args.src_language, rate=sample_rate, error_messages_callback=show_error_messages)
 
-            converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
-            recognizer = SpeechRecognizer(language=args.src_language, rate=sample_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", error_messages_callback=show_error_messages)
+        pool = multiprocessing.Pool(args.concurrency)
 
-            if regions:
+        if regions:
+            try:
                 widgets = ["Converting speech regions to FLAC files : ", Percentage(), ' ', Bar(), ' ', ETA()]
                 pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
                 extracted_regions = []
                 for i, extracted_region in enumerate(pool.imap(converter, regions)):
                     extracted_regions.append(extracted_region)
                     pbar.update(i)
                 pbar.finish()
@@ -227,134 +129,87 @@
                 pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
                 transcripts = []
                 for i, transcript in enumerate(pool.imap(recognizer, extracted_regions)):
                     transcripts.append(transcript)
                     pbar.update(i)
                 pbar.finish()
 
-                subtitle_format = args.format
-                base, ext = os.path.splitext(media_filepath)
-                subtitle_filepath = "{base}.{format}".format(base=base, format=subtitle_format)
-
-                writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                writer.write(subtitle_filepath)
-
-                if do_translate:
-                    # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
-                    # NO NEED TO TRANSLATE ALL transcript IN transcripts
-                    # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
-                    # JUST TRANSLATE ALREADY CREATED subtitles ENTRIES FROM timed_subtitles
-                    timed_subtitles = writer.timed_subtitles
-                    created_regions = []
-                    created_subtitles = []
-                    for entry in timed_subtitles:
-                        created_regions.append(entry[0])
-                        created_subtitles.append(entry[1])
-
-                    prompt = "Translating from %s to %s   : " %(args.src_language.center(8), args.dst_language.center(8))
-                    widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
-
-                    transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
-
-                    translated_subtitles = []
-                    for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
-                        translated_subtitles.append(translated_subtitle)
-                        pbar.update(i)
-                    pbar.finish()
-
-                    translated_subtitle_filepath = subtitle_filepath[ :-4] + '.translated.' + subtitle_format
-                    translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
-                    translation_writer.write(translated_subtitle_filepath)
-
-                if do_translate:
-                    print("Original subtitles file created at      : {}".format(subtitle_filepath))
-                    print("Translated subtitles file created at    : {}" .format(translated_subtitle_filepath))
-                else:
-                    print("Subtitles file created at               : {}".format(subtitle_filepath))
-
-                if args.render:
-                    base, ext = os.path.splitext(media_filepath)
-                    rendered_media_filepath = "{base}.rendered.{format}".format(base=base, format=ext[1:])
-
-                    subtitle_path = None
-                    if do_translate:
-                        subtitle_path = translated_subtitle_filepath
-                    else:
-                        subtitle_path = subtitle_filepath
-
-                    ffmpeg_language_code = language.ffmpeg_code_of_code[args.src_language]
-                    subtitle_renderer = MediaSubtitleRenderer(subtitle_path=subtitle_path, language=ffmpeg_language_code, output_path=rendered_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    widgets = [f"Rendering subtitles with {media_type}          : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    result = subtitle_renderer(media_filepath)
-                    pbar.finish()
-
-                    if result and os.path.isfile(result):
-                        print("Rendered video created at               : {}".format(rendered_media_filepath))
-
-                if not args.render:
-                    completed_tasks += 1
-                elif args.render:
-                    if rendered_media_filepath and os.path.isfile(rendered_media_filepath):
-                        completed_tasks += 1
-
-                print('')
-                if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
-                    transcribe_end_time = time.time()
-                    transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
-                    transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
-                    transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
-                    hour, minute, second = transcribe_elapsed_time_str.split(":")
-                    msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
-                    print(msg)
-
-        except KeyboardInterrupt:
-            pbar.finish()
-            pool.terminate()
-            pool.close()
-            pool.join()
-            print("Cancelling all tasks")
-
-            if sys.platform == "win32":
-                stop_ffmpeg_windows(error_messages_callback=show_error_messages)
-            else:
-                stop_ffmpeg_linux(error_messages_callback=show_error_messages)
-
-            remove_temp_files("flac")
-            remove_temp_files("wav")
-            return 1
+            except KeyboardInterrupt:
+                pbar.finish()
+                pool.terminate()
+                pool.close()
+                pool.join()
+                print("Cancelling all tasks")
+                return 1
 
-        except Exception as e:
-            if not KeyboardInterrupt in e:
+            except Exception as e:
                 pbar.finish()
                 pool.terminate()
                 pool.close()
                 pool.join()
                 print(e)
+                return 1
+
+        subtitle_filepath = args.output
+        subtitle_format = args.format
+        # HANDLE IF THERE ARE SOME TYPOS IN SUBTITLE FILENAME
+        if subtitle_filepath:
+            subtitle_file_base, subtitle_file_ext = os.path.splitext(args.output)
+            if not subtitle_file_ext:
+                subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=subtitle_format)
+            else:
+                subtitle_filepath = args.output
+        else:
+            base, ext = os.path.splitext(media_filepath)
+            subtitle_filepath = "{base}.{format}".format(base=base, format=subtitle_format)
 
-                if sys.platform == "win32":
-                    stop_ffmpeg_windows(error_messages_callback=show_error_messages)
-                else:
-                    stop_ffmpeg_linux(error_messages_callback=show_error_messages)
+        writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
+        writer.write(subtitle_filepath)
 
-                remove_temp_files("flac")
-                remove_temp_files("wav")
-                return 1
+        if do_translate:
+
+            # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
+            # NO NEED TO TRANSLATE ALL transcript IN transcripts
+            # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
+            # JUST TRANSLATE ALREADY CREATED subtitles ENTRIES FROM timed_subtitles
+            timed_subtitles = writer.timed_subtitles
+            created_regions = []
+            created_subtitles = []
+            for entry in timed_subtitles:
+                created_regions.append(entry[0])
+                created_subtitles.append(entry[1])
+
+            prompt = "Translating from %8s to %8s   : " %(args.src_language, args.dst_language)
+            widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
+            pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
+            transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
+            translated_subtitles = []
+            for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
+                translated_subtitles.append(translated_subtitle)
+                pbar.update(i)
+            pbar.finish()
 
-    if pool:
-        pool.close()
-        pool.join()
-        pool = None
+            translated_subtitle_filepath = subtitle_filepath[ :-4] + '.translated.' + subtitle_format
+            translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
+            translation_writer.write(translated_subtitle_filepath)
+
+        print('Done.')
+        if do_translate:
+            print("Original subtitles file created at      : {}".format(subtitle_filepath))
+            print('Translated subtitles file created at    : {}' .format(translated_subtitle_filepath))
+        else:
+            print("Subtitles file created at               : {}".format(subtitle_filepath))
 
     if sys.platform == "win32":
         stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
+    pool.close()
+    pool.join()
+
     remove_temp_files("flac")
     remove_temp_files("wav")
 
-
 if __name__ == '__main__':
     multiprocessing.freeze_support()
     sys.exit(main())
```

### Comparing `autosrt-1.3.4/autosrt.egg-info/PKG-INFO` & `autosrt-1.3.5/autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.4
+Version: 1.3.5
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.4/setup.py` & `autosrt-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.4/test/test1.py` & `autosrt-1.3.5/test/test1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from progressbar import ProgressBar, Percentage, Bar, ETA
 
 
 from autosrt import Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter
 
 # CREATE A progress_callback FUNCTION TO SHOW PROGRESS WHEN CONVERT TO A TEMPORARY WAV FILE
-def show_progress(progress):
+def show_progress(media_filepath, progress):
    global pbar
    pbar.update(progress)
 
 
 def show_error_messages(messages):
     print(messages)
 
@@ -84,14 +84,15 @@
     # CONVERT MEDIA FILE TO A TEMPORARY WAV FILE
 
     # CONVERT WITHOUT SHOWING THE PROGRESS
     #wav_converter = WavConverter(channels=1, rate=48000, progress_callback=None, error_messages_callback=show_error_messages)
     #wav_filepath, sample_rate = wav_converter(media_filepath)
 
     # CONVERT WITH SHOWING THE PROGRESS
+    print("media_filepath = {}".format(media_filepath))
     wav_converter = WavConverter(channels=1, rate=48000, progress_callback=show_progress, error_messages_callback=show_error_messages)
     widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
     pbar = ProgressBar(widgets=widgets, maxval=100).start()
     wav_filepath, sample_rate = wav_converter(media_filepath)
     pbar.finish()
 
     print("wav_filepath = {}".format(wav_filepath))
```

### Comparing `autosrt-1.3.4/test/test2.py` & `autosrt-1.3.5/test/test2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import multiprocessing
 from progressbar import ProgressBar, Percentage, Bar, ETA
 
 from autosrt import Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter
 
-def show_progress(percentage):
+def show_progress(media_filepath, percentage):
     global pbar
     pbar.update(percentage)
 
 def show_error_messages(messages):
     print(messages)
 
 def main():
```

### Comparing `autosrt-1.3.4/test/test4.py` & `autosrt-1.3.5/test/test4.py`

 * *Files identical despite different names*

