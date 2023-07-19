# Comparing `tmp/sparkx-1.0.0-py3-none-any.whl.zip` & `tmp/sparkx-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 64820 bytes, number of entries: 19
+Zip file size: 65100 bytes, number of entries: 19
 -rw-r--r--  2.0 unx     7006 b- defN 20-Feb-02 00:00 sparkx/EventCharacteristics.py
 -rwxr-xr-x  2.0 unx    18043 b- defN 20-Feb-02 00:00 sparkx/Histogram.py
--rwxr-xr-x  2.0 unx    14780 b- defN 20-Feb-02 00:00 sparkx/JetAnalysis.py
--rw-r--r--  2.0 unx    37090 b- defN 20-Feb-02 00:00 sparkx/Jetscape.py
+-rwxr-xr-x  2.0 unx    15267 b- defN 20-Feb-02 00:00 sparkx/JetAnalysis.py
+-rw-r--r--  2.0 unx    37096 b- defN 20-Feb-02 00:00 sparkx/Jetscape.py
 -rw-r--r--  2.0 unx    35760 b- defN 20-Feb-02 00:00 sparkx/Lattice3D.py
 -rw-r--r--  2.0 unx    45714 b- defN 20-Feb-02 00:00 sparkx/Oscar.py
 -rwxr-xr-x  2.0 unx    26671 b- defN 20-Feb-02 00:00 sparkx/Particle.py
 -rw-r--r--  2.0 unx     1580 b- defN 20-Feb-02 00:00 sparkx/Utilities.py
 -rw-r--r--  2.0 unx        2 b- defN 20-Feb-02 00:00 sparkx/__init__.py
 -rw-r--r--  2.0 unx    16349 b- defN 20-Feb-02 00:00 sparkx/flow/EventPlaneFlow.py
 -rw-r--r--  2.0 unx      358 b- defN 20-Feb-02 00:00 sparkx/flow/FlowInterface.py
 -rw-r--r--  2.0 unx    21681 b- defN 20-Feb-02 00:00 sparkx/flow/GenerateFlow.py
 -rw-r--r--  2.0 unx     6219 b- defN 20-Feb-02 00:00 sparkx/flow/ReactionPlaneFlow.py
 -rw-r--r--  2.0 unx    14059 b- defN 20-Feb-02 00:00 sparkx/flow/ScalarProductFlow.py
 -rw-r--r--  2.0 unx        2 b- defN 20-Feb-02 00:00 sparkx/flow/__init__.py
-?rw-r--r--  2.0 unx     1648 b- defN 20-Feb-02 00:00 sparkx-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sparkx-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 sparkx-1.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1505 b- defN 20-Feb-02 00:00 sparkx-1.0.0.dist-info/RECORD
-19 files, 283703 bytes uncompressed, 62404 bytes compressed:  78.0%
+?rw-r--r--  2.0 unx     1857 b- defN 20-Feb-02 00:00 sparkx-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sparkx-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 sparkx-1.0.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1505 b- defN 20-Feb-02 00:00 sparkx-1.0.1.dist-info/RECORD
+19 files, 284405 bytes uncompressed, 62684 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: sparkx/flow/ScalarProductFlow.py
 Comment: 
 
 Filename: sparkx/flow/__init__.py
 Comment: 
 
-Filename: sparkx-1.0.0.dist-info/METADATA
+Filename: sparkx-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: sparkx-1.0.0.dist-info/WHEEL
+Filename: sparkx-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: sparkx-1.0.0.dist-info/licenses/LICENSE
+Filename: sparkx-1.0.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: sparkx-1.0.0.dist-info/RECORD
+Filename: sparkx-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparkx/JetAnalysis.py

```diff
@@ -1,16 +1,19 @@
 import numpy as np
 import fastjet as fj
 import csv
 import warnings
-from Particle import Particle
+from sparkx.Particle import Particle
 
 class JetAnalysis:
     """
-    This class analyzes simulation output using the fastjet python package.
+    This class analyzes simulation output using the
+    `fastjet <https://fastjet.fr/repo/doxygen-3.4.1/>`__ python package.
+    For further information on the jet finding algorithms please have a look
+    at the documentation.
 
     Attributes
     ----------
     hadron_data_: list
         List of hadron data for each event.
     jet_R_: float
         Jet radius parameter.
@@ -316,20 +319,28 @@
             transverse momentum to write out the jet to a file.
             Values can be :code:`None`, then the lower bound is set to zero
             and the upper one to :math:`+\\infty`.
         output_filename: str
             Filename for the jet output.
         jet_algorithm: fastjet.JetAlgorithm, optional
             Jet algorithm for jet finding. Default is :code:`fastjet.antikt_algorithm`.
+
+        Notes
+        -----
+        The standard recombination scheme :code:`E_scheme` of the fastjet package is fixed here.
+
         """
         self.__initialize_and_check_parameters(hadron_data, jet_R, jet_eta_range, jet_pt_range)
         for event, hadron_data_event in enumerate(self.hadron_data_):
             new_file = False
             event_PseudoJets = self.create_fastjet_PseudoJets(hadron_data_event)
-            jet_definition = fj.JetDefinition(jet_algorithm, self.jet_R_)
+            if jet_algorithm == fj.ee_genkt_algorithm or jet_algorithm == fj.genkt_algorithm:
+                jet_definition = fj.JetDefinition(jet_algorithm, self.jet_R_, -1.0)
+            else:
+                jet_definition = fj.JetDefinition(jet_algorithm, self.jet_R_)
             jet_selector = fj.SelectorEtaRange(self.jet_eta_range_[0],self.jet_eta_range_[1])
 
             if event == 0:
                 print("jet definition is:", jet_definition)
                 print("jet selector is:", jet_selector)
                 # create a new file for the first event in the dataset
                 new_file = True
@@ -394,8 +405,8 @@
             List of associated particles for each jet in each element
             (:code:`[jet][associated_particle][column]`).
         """
         associated_particles_list = []
         for jet in self.jet_data_:
             associated_particles = jet[1:]
             associated_particles_list.append(associated_particles)
-        return associated_particles_list
+        return associated_particles_list
```

## sparkx/Jetscape.py

```diff
@@ -344,15 +344,15 @@
         file = open(self.PATH_JETSCAPE_ , 'r')
         event_output = []
 
         while True:
             line = file.readline()
             if not line:
                 break
-            elif '#' in line and 'weight' in line:
+            elif '#' in line and 'N_hadrons' in line:
                 line_str = line.replace('\n','').replace('\t',' ').split(' ')
                 event = line_str[2]
                 num_output = line_str[8]
                 event_output.append([event, num_output])
             else:
                 continue
         file.close()
@@ -948,15 +948,15 @@
         output_file : str
             Path to the output file like :code:`[output_directory]/particle_lists.dat`
 
         """
         format_jetscape = '%d %d %d %g %g %g %g'
         line_in_initial_file = open(self.PATH_JETSCAPE_,'r')
         header = line_in_initial_file.readline()
-        last_line = self.get_last_line(self.PATH_JETSCAPE_)
+        last_line = self.__get_last_line(self.PATH_JETSCAPE_)
         line_in_initial_file.close()
 
         output = open(output_file, "w")
         output.write(header)
         output.close()
 
         with open(output_file, "a") as f_out:
@@ -964,8 +964,8 @@
                 event = self.num_output_per_event_[i,0]
                 num_out = self.num_output_per_event_[i,1]
                 particle_output = np.asarray(self.particle_list()[i])
 
                 f_out.write(f'#\tEvent\t{event}\tweight\t1\tEPangle\t0\tN_hadrons\t{num_out}\n')
                 np.savetxt(f_out, particle_output, delimiter=' ', newline='\n', fmt=format_jetscape)
             f_out.write(last_line)
-        f_out.close()
+        f_out.close()
```

## Comparing `sparkx-1.0.0.dist-info/METADATA` & `sparkx-1.0.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Software Package for Analyzing Relativistic Kinematics in Collision eXperiments
 Project-URL: Repository, https://github.com/smash-transport/sparkx
 Project-URL: Bug Tracker, https://github.com/smash-transport/sparkx/issues
 Project-URL: Documentation, https://smash-transport.github.io/sparkx/
 Author-email: Hendrik Roch <roch@fias.uni-frankfurt.de>, Nils Sass <nsass@fias.uni-frankfurt.de>, Niklas Götz <goetz@fias.uni-frankfurt.de>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,23 @@
 Requires-Dist: fastjet==3.4.1.2
 Requires-Dist: matplotlib==3.7.1
 Requires-Dist: numpy==1.23.5
 Requires-Dist: particle==0.22.0
 Requires-Dist: scipy==1.10.1
 Description-Content-Type: text/markdown
 
-# SPARKX 
+<div style="float:right; margin:10px;">
+  <img align="right" src="https://github.com/smash-transport/sparkx/assets/90659054/58363f8a-2ed4-4a8f-bbb0-40f71349a338" alt="drawing" width="125"/>
+</div>
+<br>
+<br>
+
+# SPARKX
+
+
 ### Software Package for Analyzing Relativistic Kinematics in Collision eXperiments
 
 <a href="https://smash-transport.github.io/sparkx/" target="_blank">
   <img src="https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat" alt="documentation">
 </a>
 
 This package is designed to assist users of the [SMASH](https://smash-transport.github.io/) and [JETSCAPE/X-SCAPE](https://jetscape.org/) codes to analyze the output of the simulation data.
```

### html2text {}

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 2.1 Name: sparkx Version: 1.0.0 Summary: Software Package for
+Metadata-Version: 2.1 Name: sparkx Version: 1.0.1 Summary: Software Package for
 Analyzing Relativistic Kinematics in Collision eXperiments Project-URL:
 Repository, https://github.com/smash-transport/sparkx Project-URL: Bug Tracker,
 https://github.com/smash-transport/sparkx/issues Project-URL: Documentation,
 https://smash-transport.github.io/sparkx/ Author-email: Hendrik Roch
 fias.uni-frankfurt.de>, Nils Sass
 fias.uni-frankfurt.de>, Niklas GÃ¶tz
 fias.uni-frankfurt.de> License-File: LICENSE Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering Requires-Python: >=3.7 Requires-Dist: abc-property==1.0
 Requires-Dist: fastjet==3.4.1.2 Requires-Dist: matplotlib==3.7.1 Requires-Dist:
 numpy==1.23.5 Requires-Dist: particle==0.22.0 Requires-Dist: scipy==1.10.1
-Description-Content-Type: text/markdown # SPARKX ### Software Package for
-Analyzing Relativistic Kinematics in Collision eXperiments [documentation] This
-package is designed to assist users of the [SMASH](https://smash-
-transport.github.io/) and [JETSCAPE/X-SCAPE](https://jetscape.org/) codes to
-analyze the output of the simulation data. It contains multiple classes to read
-in the simulation outputs in OSCAR2013/OSCAR2013Extended format or the hadron
-output of JETSCAPE/X-SCAPE.
+Description-Content-Type: text/markdown
+[drawing]
+
+
+# SPARKX ### Software Package for Analyzing Relativistic Kinematics in
+Collision eXperiments [documentation] This package is designed to assist users
+of the [SMASH](https://smash-transport.github.io/) and [JETSCAPE/X-SCAPE]
+(https://jetscape.org/) codes to analyze the output of the simulation data. It
+contains multiple classes to read in the simulation outputs in OSCAR2013/
+OSCAR2013Extended format or the hadron output of JETSCAPE/X-SCAPE.
```

## Comparing `sparkx-1.0.0.dist-info/licenses/LICENSE` & `sparkx-1.0.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `sparkx-1.0.0.dist-info/RECORD` & `sparkx-1.0.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 sparkx/EventCharacteristics.py,sha256=uZc11CUzYV0dRlGrlhQE8rF8ii46O0GXTBOgtdnCCfs,7006
 sparkx/Histogram.py,sha256=KHcBlnxNJoK81oqJIpWDMNqZ9JQ2bvN9zmFBGc-vYfo,18043
-sparkx/JetAnalysis.py,sha256=t88vu5rNOPB3BQ1FBsSJmu14udxDI6N-4ShXSc4AUCc,14780
-sparkx/Jetscape.py,sha256=BRhcXmDW6gSe72j0e8hfT5l1f-G6So1HPaEfFGtGpLg,37090
+sparkx/JetAnalysis.py,sha256=LkrSI0ZiOCsjSaRMunpsgJNjMKsdL9WQF-ghVCGTG7E,15267
+sparkx/Jetscape.py,sha256=1sfWKs6AOVZ5Cd1mZyPRFwu7UP5Ly8DyomFXwasGMEA,37096
 sparkx/Lattice3D.py,sha256=x0-IvNzqlwxUE6nQzKxoPMNvqSMPhGYTwzz1QwIUdlI,35760
 sparkx/Oscar.py,sha256=tlFO1aQw4-2phHFvh9I0qAC1kbs14JehAdrtzpdU-oE,45714
 sparkx/Particle.py,sha256=nUCSyELoo2Ua5GQMJeD1n4zlYVWRfi780WhzPFvt8R0,26671
 sparkx/Utilities.py,sha256=ehyKkP1xg6zBvbo6wklIydjWUGx1iNWwQ2B8LzkANFo,1580
 sparkx/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
 sparkx/flow/EventPlaneFlow.py,sha256=Se_cvuoOYt2WXN7a1x-SzceMeK37Y7rn1AFvg44qHeA,16349
 sparkx/flow/FlowInterface.py,sha256=_k-64LLc0tts3yvwzJskRmgz1oilVd4Kw14nxYKLgw0,358
 sparkx/flow/GenerateFlow.py,sha256=ptHxiFh3CRXZ2MIp4CovUO1cvVrcd8kIVv5Ou_Dydjc,21681
 sparkx/flow/ReactionPlaneFlow.py,sha256=k1lCJVn1v7IhYjDZamFb1xXwTPeAl1S9u26SsggTLPQ,6219
 sparkx/flow/ScalarProductFlow.py,sha256=SngCQinlxfsik2kbZXnRWRrGQBNPb6HUwb35iXV8AhE,14059
 sparkx/flow/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
-sparkx-1.0.0.dist-info/METADATA,sha256=gtHJahWpjFkHiUFWNacRM0t_9_Bt9RqGgv-RkVAWXiQ,1648
-sparkx-1.0.0.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-sparkx-1.0.0.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-sparkx-1.0.0.dist-info/RECORD,,
+sparkx-1.0.1.dist-info/METADATA,sha256=kFa0_5ePL7scMXGiNERWrF9R4NUPRg5QYj44zOJ5fZE,1857
+sparkx-1.0.1.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+sparkx-1.0.1.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+sparkx-1.0.1.dist-info/RECORD,,
```

