# Comparing `tmp/gromologist-0.251.tar.gz` & `tmp/gromologist-0.252.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gromologist-0.251.tar", last modified: Fri Mar 17 14:26:16 2023, max compression
+gzip compressed data, was "gromologist-0.252.tar", last modified: Tue Jun  6 15:55:48 2023, max compression
```

## Comparing `gromologist-0.251.tar` & `gromologist-0.252.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mwieczor  (1000) mwieczor  (1000)        0 2023-03-17 14:26:16.474961 gromologist-0.251/
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    35059 2022-08-11 14:28:45.000000 gromologist-0.251/LICENSE
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      241 2023-03-17 14:26:16.474961 gromologist-0.251/PKG-INFO
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    28407 2023-02-03 15:20:24.000000 gromologist-0.251/README.md
-drwxrwxr-x   0 mwieczor  (1000) mwieczor  (1000)        0 2023-03-17 14:26:16.470961 gromologist-0.251/gromologist/
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    25991 2022-08-16 11:53:50.000000 gromologist-0.251/gromologist/Crooks.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    21145 2022-08-11 14:28:45.000000 gromologist-0.251/gromologist/DihOpt.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    18412 2023-02-28 18:04:10.000000 gromologist-0.251/gromologist/Entries.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    22539 2023-03-01 21:58:22.000000 gromologist-0.251/gromologist/Gmx.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    19635 2023-03-14 18:59:23.000000 gromologist-0.251/gromologist/Mutant.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)     8520 2023-03-14 18:49:05.000000 gromologist-0.251/gromologist/Parser.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    68545 2023-03-14 19:23:43.000000 gromologist-0.251/gromologist/Pdb.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)   100116 2023-03-17 13:35:51.000000 gromologist-0.251/gromologist/Section.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    35528 2023-02-28 18:44:32.000000 gromologist-0.251/gromologist/Subsection.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    35009 2023-02-15 15:05:06.000000 gromologist-0.251/gromologist/ThDiff.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    34907 2023-03-15 22:24:52.000000 gromologist-0.251/gromologist/Topology.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)     6248 2023-03-17 13:45:54.000000 gromologist-0.251/gromologist/Utils.py
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      640 2023-02-26 22:49:14.000000 gromologist-0.251/gromologist/__init__.py
-drwxrwxr-x   0 mwieczor  (1000) mwieczor  (1000)        0 2023-03-17 14:26:16.474961 gromologist-0.251/gromologist.egg-info/
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      241 2023-03-17 14:26:16.000000 gromologist-0.251/gromologist.egg-info/PKG-INFO
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      489 2023-03-17 14:26:16.000000 gromologist-0.251/gromologist.egg-info/SOURCES.txt
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)        1 2023-03-17 14:26:16.000000 gromologist-0.251/gromologist.egg-info/dependency_links.txt
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)        1 2022-11-02 19:21:30.000000 gromologist-0.251/gromologist.egg-info/not-zip-safe
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)       12 2023-03-17 14:26:16.000000 gromologist-0.251/gromologist.egg-info/top_level.txt
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)       38 2023-03-17 14:26:16.474961 gromologist-0.251/setup.cfg
--rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      305 2023-03-17 14:25:44.000000 gromologist-0.251/setup.py
+drwxrwxr-x   0 mwieczor  (1000) mwieczor  (1000)        0 2023-06-06 15:55:48.081721 gromologist-0.252/
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    35059 2022-08-11 14:28:45.000000 gromologist-0.252/LICENSE
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      241 2023-06-06 15:55:48.081721 gromologist-0.252/PKG-INFO
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    28407 2023-02-03 15:20:24.000000 gromologist-0.252/README.md
+drwxrwxr-x   0 mwieczor  (1000) mwieczor  (1000)        0 2023-06-06 15:55:48.081721 gromologist-0.252/gromologist/
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    25991 2022-08-16 11:53:50.000000 gromologist-0.252/gromologist/Crooks.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    21145 2022-08-11 14:28:45.000000 gromologist-0.252/gromologist/DihOpt.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    18412 2023-02-28 18:04:10.000000 gromologist-0.252/gromologist/Entries.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    24106 2023-04-24 15:37:05.000000 gromologist-0.252/gromologist/Gmx.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    19635 2023-03-14 18:59:23.000000 gromologist-0.252/gromologist/Mutant.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)     8520 2023-03-14 18:49:05.000000 gromologist-0.252/gromologist/Parser.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    69420 2023-05-07 15:45:37.000000 gromologist-0.252/gromologist/Pdb.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)   100116 2023-03-17 13:35:51.000000 gromologist-0.252/gromologist/Section.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    36021 2023-03-25 20:04:33.000000 gromologist-0.252/gromologist/Subsection.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    38351 2023-05-25 15:35:18.000000 gromologist-0.252/gromologist/ThDiff.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)    34907 2023-03-15 22:24:52.000000 gromologist-0.252/gromologist/Topology.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)     6248 2023-03-17 13:45:54.000000 gromologist-0.252/gromologist/Utils.py
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      640 2023-02-26 22:49:14.000000 gromologist-0.252/gromologist/__init__.py
+drwxrwxr-x   0 mwieczor  (1000) mwieczor  (1000)        0 2023-06-06 15:55:48.081721 gromologist-0.252/gromologist.egg-info/
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      241 2023-06-06 15:55:47.000000 gromologist-0.252/gromologist.egg-info/PKG-INFO
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      489 2023-06-06 15:55:48.000000 gromologist-0.252/gromologist.egg-info/SOURCES.txt
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)        1 2023-06-06 15:55:47.000000 gromologist-0.252/gromologist.egg-info/dependency_links.txt
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)        1 2022-11-02 19:21:30.000000 gromologist-0.252/gromologist.egg-info/not-zip-safe
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)       12 2023-06-06 15:55:47.000000 gromologist-0.252/gromologist.egg-info/top_level.txt
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)       38 2023-06-06 15:55:48.081721 gromologist-0.252/setup.cfg
+-rw-rw-r--   0 mwieczor  (1000) mwieczor  (1000)      305 2023-06-06 15:55:39.000000 gromologist-0.252/setup.py
```

### Comparing `gromologist-0.251/LICENSE` & `gromologist-0.252/LICENSE`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/README.md` & `gromologist-0.252/README.md`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/Crooks.py` & `gromologist-0.252/gromologist/Crooks.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/DihOpt.py` & `gromologist-0.252/gromologist/DihOpt.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/Entries.py` & `gromologist-0.252/gromologist/Entries.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/Gmx.py` & `gromologist-0.252/gromologist/Gmx.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,42 +164,50 @@
     :return: int, number of frames found
     """
     output = gml.gmx_command(gmx, 'check', f=trajfile, answer=True).split('\n')
     return [int(x.split()[1]) for x in output if len(x.split()) > 1 and x.split()[0] == "Coords"][0]
 
 
 def calc_gmx_energy(struct: str, topfile: str, gmx: str = '', quiet: bool = False, traj: Optional[str] = None,
-                    terms: str = 'potential', cleanup: bool = True, group_a: Optional[str] = None,
-                    group_b: Optional[str] = None) -> dict:
+                    terms: Optional[Union[str, list]] = None, cleanup: bool = True, group_a: Optional[str] = None,
+                    group_b: Optional[str] = None, sum_output: bool = False, savetxt: Optional[str] = None) -> dict:
     """
     Calculates selected energy terms given a structure/topology pair or structure/topology/trajectory set.
     :param struct: str, path to the structure file
     :param topfile: str, path to the topology file
     :param gmx: str, path to the gmx executable (if not found in the $PATH)
     :param quiet: bool, whether to print gmx output to the screen
     :param traj: str, path to the trajectory (optional)
     :param terms: str or list, terms which will be calculated according to gmx energy naming (can also be "all")
     :param cleanup: bool, whether to remove intermediate files (useful for debugging)
     :param group_a: str, selection defining group A to calculate interactions between group A and B
     :param group_b: str, selection defining group B to calculate interactions between group A and B
+    :param sum_output: bool, whether to add a term "sum" that will contain all terms added up
     :return: dict of lists, one list of per-frame values per each selected term
     """
     if not gmx:
         gmx = os.popen('which gmx 2> /dev/null').read().strip()
     if not gmx:
         gmx = os.popen('which gmx_mpi 2> /dev/null').read().strip()
     if not gmx:
         gmx = os.popen('which gmx_d 2> /dev/null').read().strip()
+    if (group_b or group_a) and not (group_a and group_b):
+        raise RuntimeError("If you're choosing individual groups, please specify both group_a and group_b")
     if group_a and group_b:
         group_names = ndx(gml.Pdb(struct), [group_a, group_b, 'all'])
         gen_mdp('rerun.mdp', energygrps=f"{group_names[0]} {group_names[1]} ")
         gmx_command(gmx, 'grompp', quiet=quiet, f='rerun.mdp', p=topfile, c=struct, o='rerun', maxwarn=5, n='gml.ndx')
+        if terms is None:
+            terms = ['coul-sr:g1-g2', 'lj-sr:g1-g2']
+            sum_output = True
     else:
         gen_mdp('rerun.mdp')
         gmx_command(gmx, 'grompp', quiet=quiet, f='rerun.mdp', p=topfile, c=struct, o='rerun', maxwarn=5)
+        if terms is None:
+            terms = 'potential'
     gmx_command(gmx, 'mdrun', quiet=quiet, deffnm='rerun', rerun=struct if traj is None else traj)
     legend = get_legend(gmx, 'rerun.edr')
     if terms == 'all':
         terms = list(legend.keys())
     if isinstance(terms, str):
         terms = [terms]
     try:
@@ -210,15 +218,27 @@
     out = read_xvg('energy.xvg')
     if cleanup:
         to_remove = ['rerun.mdp', 'mdout.mdp', 'rerun.tpr', 'rerun.trr', 'rerun.edr', 'rerun.log', 'energy.xvg']
         if group_a and group_b:
             to_remove.append('gml.ndx')
         for filename in to_remove:
             os.remove(filename)
-    return {term: [o[onum] for o in out] for term, onum in zip(terms, range(len(out[0])))}
+    values = {term: [o[onum] for o in out] for term, onum in zip(terms, range(len(out[0])))}
+    if sum_output:
+        nframes = len(values[list(values.keys())[0]])
+        values['sum'] = [sum([values[k][n] for k in values.keys()]) for n in range(nframes)]
+    if savetxt is not None:
+        nframes = len(values[list(values.keys())[0]])
+        header = ' '.join(values.keys())
+        entries = [' '.join([f"{values[k][n]:12.5f}" for k in values.keys()]) for n in range(nframes)]
+        with open(savetxt, 'w') as out:
+            out.write(header + '\n')
+            for ent in entries:
+                out.write(ent + '\n')
+    return values
 
 
 def calc_gmx_dhdl(struct: str, topfile: str, traj: str, gmx: str = '', quiet: bool = False,
                   cleanup: bool = True, **kwargs) -> list:
     """
     Calculates selected energy terms given a structure/topology pair or structure/topology/trajectory set.
     :param struct: str, path to the structure file
@@ -265,79 +285,83 @@
     print(f"Topology 1 has energy {en1}, topology 2 has energy {en2}")
     return en1 == en2
 
 
 def prepare_system(struct: str, ff: Optional[str] = None, water: Optional[str] = None,
                    box: Optional[str] = 'dodecahedron', box_margin: Optional[float] = 1.5, cation: Optional[str] = 'K',
                    anion: Optional[str] = 'CL', ion_conc: Optional[float] = 0.15, maxsol: Optional[int] = None,
-                   resize_box=True):
+                   resize_box=True, quiet=True):
     """
     Implements a full system preparation workflow (parsing the structure with pdb2gmx,
     setting the box size, adding solvent and ions, minimizing, generating a final
     merged topology + structure with added chains)
     :param struct: str, path to the structure file
     :param ff: str, name of the force field to be chosen (by default interactive)
     :param water: str, name of the water model to be used
     :param box: str, box type (default is dodecahedron)
     :param box_margin: float, box margin passed to editconf to set box size (default is 1.5 nm)
     :param cation: str, the cation to be used (default is K)
     :param anion: str, the anion to be used (default is CL)
     :param ion_conc: float, the ion concentration to be applied (default 0.15)
     :param resize_box: bool, whether to generate a new box size based on the -d option of gmx editconf
+    :param quiet: bool, whether to print gmx output to the screen
     :return: None
     """
     gmx = gml.find_gmx_dir()
     found = [f'{i} (local)' for i in glob(f'*ff')] + glob(f'{gmx[0]}/*ff')
+    if set(glob(f'*ff')).intersection(glob(f'{gmx[0]}/*ff')):
+        raise RuntimeError(f"Directories {set(glob(f'*ff')).intersection(glob(f'{gmx[0]}/*ff'))} have identical names,"
+                           f"please make them unambiguous e.g. by renaming the local version")
     if ff is None:
         for n, i in enumerate(found):
             print('[', n + 1, '] ', i.split('/')[-1])
         rtpnum = input('\nPlease select the force field:\n')
         try:
             rtpnum = int(rtpnum)
         except ValueError:
             raise RuntimeError('Not an integer: {}'.format(rtpnum))
         else:
             ff = found[rtpnum - 1].replace(' (local)', '').split('/')[-1]
-    if ff not in [i.split('/')[-1] for i in found]:
+    if ff not in [i.replace(' (local)', '').split('/')[-1] for i in found]:
         raise RuntimeError(
             f"Force field {ff.split('/')[-1]} not found in the list: {[i.split('/')[-1] for i in found]}")
     ff = ff.replace('.ff', '')
     if water is None:
         water = \
         [line.split()[0] for line in open(found[rtpnum - 1].replace(' (local)', '') + os.sep + 'watermodels.dat')
          if 'recommended' in line][0]
-    print(gmx_command(gmx[1], 'pdb2gmx', quiet=False, f=struct, ff=ff, water=water,
-                      answer=True, fail_on_error=True))
+    gmx_command(gmx[1], 'pdb2gmx', quiet=quiet, f=struct, ff=ff, water=water,
+                      answer=True, fail_on_error=True)
     if resize_box:
-        print(gmx_command(gmx[1], 'editconf', f='conf.gro', o='box.gro', d=box_margin, bt=box,
-                          answer=True, fail_on_error=True))
+        gmx_command(gmx[1], 'editconf', f='conf.gro', o='box.gro', d=box_margin, bt=box, quiet=quiet,
+                          answer=True, fail_on_error=True)
     else:
         copy2('conf.gro', 'box.gro')
     if maxsol is None:
-        print(gmx_command(gmx[1], 'solvate', cp='box.gro', p='topol.top', o='water.gro',
-                          answer=True, fail_on_error=True))
+        gmx_command(gmx[1], 'solvate', cp='box.gro', p='topol.top', o='water.gro', quiet=quiet,
+                          answer=True, fail_on_error=True)
     else:
-        print(gmx_command(gmx[1], 'solvate', cp='box.gro', p='topol.top', o='water.gro', maxsol=maxsol,
-                          answer=True, fail_on_error=True))
+        gmx_command(gmx[1], 'solvate', cp='box.gro', p='topol.top', o='water.gro', maxsol=maxsol, quiet=quiet,
+                          answer=True, fail_on_error=True)
     gen_mdp('do_minimization.mdp', runtype='mini')
-    print(gmx_command(gmx[1], 'grompp', f='do_minimization.mdp', p='topol.top', c='water.gro', o='ions', maxwarn=1,
-                      answer=True, fail_on_error=True))
+    gmx_command(gmx[1], 'grompp', f='do_minimization.mdp', p='topol.top', c='water.gro', o='ions', maxwarn=1,
+                      quiet=quiet, answer=True, fail_on_error=True)
     answer = gmx_command(gmx[1], 'genion', pass_values=['a'], s='ions', pname=cation, nname=anion, conc=ion_conc,
-                         neutral=True, p="topol", o='test', answer=True)
+                         quiet=quiet, neutral=True, p="topol", o='test', answer=True)
     sol = int([line.split()[1] for line in answer.split('\n') if 'SOL' in line][0])
-    print(gmx_command(gmx[1], 'genion', pass_values=[sol], s='ions', pname=cation, nname=anion, conc=ion_conc,
-                      neutral=True, p="topol", o='ions', answer=True, fail_on_error=True))
-    print(gmx_command(gmx[1], 'grompp', f='do_minimization.mdp', p='topol.top', c='ions.gro', o='do_mini',
-                      answer=True, fail_on_error=True))
-    print(gmx_command(gmx[1], 'mdrun', deffnm='do_mini', v=True,
-                      answer=True, fail_on_error=True))
+    gmx_command(gmx[1], 'genion', pass_values=[sol], s='ions', pname=cation, nname=anion, conc=ion_conc,
+                      quiet=quiet, neutral=True, p="topol", o='ions', answer=True, fail_on_error=True)
+    gmx_command(gmx[1], 'grompp', f='do_minimization.mdp', p='topol.top', c='ions.gro', o='do_mini',
+                      quiet=quiet, answer=True, fail_on_error=True)
+    gmx_command(gmx[1], 'mdrun', deffnm='do_mini', v=True,
+                      quiet=quiet, answer=True, fail_on_error=True)
     ndx(gml.Pdb('do_mini.gro'), selections=['all', 'not solvent'])
-    print(gmx_command(gmx[1], 'trjconv', s='do_mini.tpr', f='do_mini.gro', o='whole.gro', pbc='cluster',
-                      pass_values=[1, 0],
-                      n='gml.ndx', answer=True, fail_on_error=True))
+    gmx_command(gmx[1], 'trjconv', s='do_mini.tpr', f='do_mini.gro', o='whole.gro', pbc='cluster',
+                      pass_values=[1, 0], quiet=quiet,
+                      n='gml.ndx', answer=True, fail_on_error=True)
     t = gml.Top('topol.top')
     t.clear_sections()
     t.save_top('merged_topology.top')
     p = gml.Pdb('whole.gro', top=t)
     p.add_chains()
     p.save_pdb('minimized_structure.pdb')
 
@@ -438,14 +462,15 @@
     :return: None
     """
     gmx = gml.find_gmx_dir()
     groups = get_groups(tpr) if ndx is None else get_groups(ndx=ndx)
     outgroup = groups[group_output]
     clustgroup = groups[group_cluster]
     passvals = [clustgroup, outgroup] if pbc == 'cluster' else [outgroup]
+    # TODO dump clustered solute, find COM, center it, cluster/res again?
     for traj in glob(mask):
         if ndx is not None:
             gmx_command(gmx[1], 'trjconv', s=tpr, f=traj, o=f'whole_{traj}', pbc=pbc, pass_values=passvals,
                         n=ndx, answer=False, fail_on_error=True)
         else:
             gmx_command(gmx[1], 'trjconv', s=tpr, f=traj, o=f'whole_{traj}', pbc=pbc, pass_values=passvals,
                         answer=False, fail_on_error=True)
```

### Comparing `gromologist-0.251/gromologist/Mutant.py` & `gromologist-0.252/gromologist/Mutant.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/Parser.py` & `gromologist-0.252/gromologist/Parser.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/Pdb.py` & `gromologist-0.252/gromologist/Pdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,19 @@
 
     @property
     def natoms(self) -> int:
         return len(self.atoms)
 
     @property
     def chains(self) -> list:
-        return sorted({a.chain for a in self.atoms})
+        chns = []
+        for a in self.atoms:
+            if a.chain not in chns:
+                chns.append(a.chain)
+        return chns
 
     @classmethod
     def from_selection(cls, pdb: "gml.Pdb", selection: str) -> "gml.Pdb":
         """
         Creates a new Pdb instance as a subset of an existing one,
         given a selection that defines a subset of atoms
         :param pdb: Pdb instance, source structure
@@ -328,14 +332,33 @@
         if atom_entry.atomname != atom_instance.atomname or atom_entry.resname != atom_instance.resname:
             print("Atoms {} ({}/{}) in molecule {} topology and {} ({}/{}) in .pdb have "
                   "non-matching names".format(atom_entry.num, atom_entry.atomname, atom_entry.resname, mol_name,
                                               atom_instance.serial, atom_instance.atomname, atom_instance.resname))
             return 1
         return 0
 
+    def permute_chains(self, permute: list, rename: bool = True):
+        """
+        Permutes the atoms in a molecule so that the order of chain is altered
+        :param permute: list, target permutation (0-based)
+        :param rename: bool, whether to adjust chain names after the permutation
+        :return: None
+        """
+        assert sorted(permute) == list(range(len(permute)))
+        assert len(self.chains) == len(permute)
+        new_atoms = []
+        for chnr in permute:
+            chname = self.chains[chnr]
+            new_atoms.extend(self.get_atoms(f'chain {chname}'))
+        new_atoms.extend(self.get_atoms(f'not chain {" ".join(self.chains)}'))
+        if rename:
+            self.renumber_atoms()
+            self.add_chains()
+        self.atoms = new_atoms
+
     def print_mols(self):
         """
         Identifies and lists molecules contained in the structure, chain by chain
         :return: None
         """
         # TODO fix
         chains = list({a.chain.strip() for a in self.atoms})
```

### Comparing `gromologist-0.251/gromologist/Section.py` & `gromologist-0.252/gromologist/Section.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/Subsection.py` & `gromologist-0.252/gromologist/Subsection.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,14 +518,26 @@
         if not isinstance(other, SubsectionParam):
             raise TypeError("{} is not a SubsectionParam instance".format(other))
         if self.header != other.header:
             raise TypeError("Cannot merge subsections with different headers: {} and {}".format(self.header,
                                                                                                 other.header))
         return SubsectionParam(["[ {} ]\n".format(self.header)] + self.entries + other.entries, self.section)
 
+    def get_entries_by_types(self, *types):
+        found = []
+        for entry in self.entries_param:
+            if len(types) != len(entry.types):
+                continue
+            if all([query == tp for query, tp in zip(types, entry.types)]) \
+                    or all([query == tp for query, tp in zip(types, entry.types[::-1])]):
+                found.append(entry)
+        if not found:
+            raise RuntimeError(f"No entry found with types: {types}")
+        return found
+
     @property
     def entries_param(self):
         return [e for e in self.entries if isinstance(e, gml.EntryParam)]
 
     def sort(self):
         """
         In case we want to sort entries after some are added at the end of the section
```

### Comparing `gromologist-0.251/gromologist/ThDiff.py` & `gromologist-0.252/gromologist/ThDiff.py`

 * *Files 3% similar despite different names*

```diff
@@ -337,38 +337,48 @@
         for atomset in self.atoms:
             ok = all([atom.type == atomset[0].type for atom in atomset])
             if not ok:
                 raise ValueError("atoms within a single parameter modification need to have consistent types")
 
 
 class ThermoDiff:
+    """
+    PLEASE NOTE: certain box types are not suitable for reruns in Gromacs
+    (e.g. Amber periodic octahedron). If that's your case, make sure your
+    molecules are whole, and use an external tool (e.g. MDTraj) to edit
+    your box angles and box side lengths to ensure sufficient space between
+    periodic images (PME is not used in reruns anyway, just plain cut-off).
+    """
     def __init__(self, temperature=300):
         self.mods = []
         self.temperature = temperature
         self.trajs = []
         self.path = None
         self.derivatives = {}
         self.discrete_free_energy_derivatives = {}
         self.profile_free_energy_derivatives = {}
         self.discrete_observable_derivatives = {}
         self.profile_observable_derivatives = {}
+        self.thresholds = {}
 
-    def add_mod(self, top: Union[str, gml.Top], structure: str, modtype: str, selections: list):
+    def add_mod(self, top: Union[str, gml.Top], structure: str, modtype: str, selections: list,
+                period: Optional[int] = -1):
         """
         Adds a new modified topology for derivative calculation
         :param top: str or gml.Top, the topology compatible with the system
         :param structure: str, a path to the Pdb or Gro file
         :param modtype: str, type of the modification, one of the following: c, s, e, n, m, a, d
         :param selections: list of str, selections that will define atoms to be modified
+        :param period: int, periodicity for a dihedral modification (if applicable)
         :return: None
         """
         if modtype in 'cse':
             self.mods.append(ModAtom(top, structure, selections, modtype))
         elif modtype in 'ad':
-            self.mods.append(ModParam(top, structure, selections, modtype))
+            self.mods.append(ModParam(top, structure, selections, modtype, period))
         elif modtype in 'nm':
             self.mods.append(ModNbfix(top, structure, selections, modtype))
 
     def add_all_nbfix_mods(self, top: Union[str, gml.Top], structure: str):
         topology = gml.Top(top) if isinstance(top, str) else top
         topology.clear_sections()
         topology.clear_ff_params()
@@ -381,14 +391,41 @@
 
     def add_all_sigma_mods(self, top: Union[str, gml.Top], structure: str, exclude: Optional[list] = None):
         self._add_lj_mods(top, structure, 'sigma', exclude)
 
     def add_all_epsilon_mods(self, top: Union[str, gml.Top], structure: str, exclude: Optional[list] = None):
         self._add_lj_mods(top, structure, 'epsilon', exclude)
 
+    def add_all_dihedral_mods(self, top: Union[str, gml.Top], structure: str, molecules: Optional[list] = None,
+                              selector_type: Optional[str] = None):
+        topology = gml.Top(top) if isinstance(top, str) else top
+        topology.clear_sections()
+        topology.clear_ff_params()
+        topology.add_ff_params()
+        topology.explicit_defines()
+        mols = topology.molecules if molecules is None else [topology.get_molecule(x) for x in molecules]
+        dihtypes = []
+        for mol in mols:
+            try:
+                sub = mol.get_subsection('dihedrals')
+            except KeyError:
+                continue
+            for dih_entry in sub.entries_bonded:
+                dih_entry.read_types()
+                signature = (dih_entry.types_state_a, dih_entry.params_state_a[-1])
+                signature_rev = (dih_entry.types_state_a[::-1], dih_entry.params_state_a[-1])
+                if signature not in dihtypes and signature_rev not in dihtypes:
+                    dihtypes.append(signature)
+        if selector_type is not None:
+            dihtypes = [d for d in dihtypes if selector_type in d[0]]
+        for n, dih in enumerate(dihtypes):
+            sels = [f'type {t}' for t in dih[0]]
+            print(f"Adding modification: {', '.join(sels)}, {n}/{len(dihtypes)}")
+            self.add_mod(deepcopy(topology), structure, 'd', sels, dih[1])
+
     def _add_lj_mods(self, top: Union[str, gml.Top], structure: str, which: str, exclude: Optional[list] = None):
         """
         Automatically adds calculations of derivatives with respect to
         all sigma or epsilon values in the system at hand
         :param top: either str (filename) or gml.Top instance
         :param structure: str, filename of the .pdb or .gro corresponding to the .top file
         :param which: str, 'sigma' or 'epsilon'
@@ -486,14 +523,15 @@
             except FileExistsError:
                 pass
             mod.save_mod(f'{self.path}/working/{str(mod)}', str(mod))
 
     def launch_reruns(self):
         """
         Launches reruns for each legal mod-trajectory combination
+        :param nproc: int, optional number of processes
         :return: None
         """
         pairs = []
         for mod in self.mods:
             for traj in self.trajs:
                 if self.equal_tops(mod.top, traj['top']):
                     datasets = self.get_traj(traj['id'])['datasets']
@@ -628,14 +666,15 @@
             if len(threshold) % 2 == 1:
                 raise RuntimeError("The list 'threshold' has to have an even number of entries, one for each starting "
                                    "and ending point of each state")
         states = [(round(x, 6), round(y, 6)) for x, y in
                   zip(threshold[::2], threshold[1::2])] if threshold is not None else \
             sorted(list({data for traj in self.trajs for data in traj['datasets'][dataset]}))
         binning_dset, deriv_dset = (dataset, dataset) if cv_dataset is None else (cv_dataset, dataset)
+        self.thresholds[dataset] = threshold
         for mod in self.mods:
             binning_data, deriv_data, weights, derivs = self.get_flat_data(binning_dset, deriv_dset, mod)
             mean_derivatives = {st: 0 for st in states + [None]}
             mean_product = {st: 0 for st in states + [None]}
             mean_data = {st: 0 for st in states + [None]}
             counter = {st: 0 for st in states + [None]}
             for n in range(len(binning_data)):
@@ -713,7 +752,32 @@
         """
         derivs = self.discrete_free_energy_derivatives if free_energy else self.discrete_observable_derivatives
         for key in derivs.keys():
             if key[1] == dataset:
                 mod = key[0]
                 with open(f'working/{mod}/{key[1]}-discrete_sensitivity.dat', 'w') as outfile:
                     outfile.write(f"{round(derivs[key][1] - derivs[key][0], 3)}\n")
+
+    def print_discrete_derivatives(self, dataset: str, free_energy: bool):
+        derivs = self.discrete_free_energy_derivatives if free_energy else self.discrete_observable_derivatives
+        thrs = self.thresholds[dataset]
+        for x in range(len(thrs)//2):
+            x1 = round(thrs[2 * x], 3)
+            x2 = round(thrs[2 * x + 1], 3)
+            xx = f"{x1}-{x2}"
+            print(f'  {xx:20s}', end='|')
+        print(f'{"  others":20s}  |')
+        print(23 * (len(thrs)//2 + 1) * '-')
+        all_ders = [q for q in derivs.keys() if q[1] == dataset]
+        sorted_ders = sorted(all_ders, key=lambda l: abs(derivs[l][1] - derivs[l][0]), reverse=True)
+        strings = {}
+        for n, mod in enumerate(all_ders):
+            strings[mod] = []
+            for d in derivs[mod]:
+                strings[mod].append(f'  {d-derivs[mod][0]:20.5f}|')
+            try:
+                strings[mod].append(f"  {str(self.mods[n]):6s}  {'-'.join(self.mods[n].types):16s}  {self.mods[n].period:4d}\n")
+            except:
+                strings[mod].append(f"  {str(self.mods[n]):6s}  {'-'.join(self.mods[n].types):16s}\n")
+            strings[mod].append(23 * (len(thrs)//2 + 1) * '-')
+        for sormod in sorted_ders:
+            print(''.join(strings[sormod]))
```

### Comparing `gromologist-0.251/gromologist/Topology.py` & `gromologist-0.252/gromologist/Topology.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/Utils.py` & `gromologist-0.252/gromologist/Utils.py`

 * *Files identical despite different names*

### Comparing `gromologist-0.251/gromologist/__init__.py` & `gromologist-0.252/gromologist/__init__.py`

 * *Files identical despite different names*

