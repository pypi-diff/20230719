# Comparing `tmp/AlleleFinder-0.1.3.tar.gz` & `tmp/AlleleFinder-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamkoziol/PycharmProjects/AlleleFinder/dist/tmpafl07hzr/AlleleFinder-0.1.3.tar", last modified: Mon Jun 19 18:23:23 2023, max compression
+gzip compressed data, was "/home/adamkoziol/PycharmProjects/AlleleFinder/dist/tmphdawvaw0/AlleleFinder-0.1.4.tar", last modified: Wed Jul 19 14:35:17 2023, max compression
```

## Comparing `AlleleFinder-0.1.3.tar` & `AlleleFinder-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/
--rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)     1113 2023-02-24 20:49:53.000000 AlleleFinder-0.1.3/setup.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1077 2023-03-10 15:09:59.000000 AlleleFinder-0.1.3/LICENSE
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/PKG-INFO
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      742 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       19 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/top_level.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/PKG-INFO
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     8402 2023-06-01 18:07:22.000000 AlleleFinder-0.1.3/README.md
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/allele_tools/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    24429 2023-03-24 14:27:36.000000 AlleleFinder-0.1.3/allele_tools/allele_profiler.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35564 2023-06-19 15:26:07.000000 AlleleFinder-0.1.3/allele_tools/stec.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-06-22 16:34:50.000000 AlleleFinder-0.1.3/allele_tools/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6368 2023-03-13 14:59:24.000000 AlleleFinder-0.1.3/allele_tools/profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    96996 2023-06-19 16:12:53.000000 AlleleFinder-0.1.3/allele_tools/methods.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       51 2023-06-19 16:18:22.000000 AlleleFinder-0.1.3/allele_tools/version.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    28340 2023-03-24 18:52:09.000000 AlleleFinder-0.1.3/allele_tools/allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35343 2023-03-24 19:36:21.000000 AlleleFinder-0.1.3/allele_tools/allele_translate_reduce.py
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/tests/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4680 2023-06-19 16:07:38.000000 AlleleFinder-0.1.3/tests/test_5_stec_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6584 2023-06-01 15:06:40.000000 AlleleFinder-0.1.3/tests/test_1_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4628 2023-03-13 20:02:00.000000 AlleleFinder-0.1.3/tests/test_3_stec_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2107 2023-06-19 16:16:44.000000 AlleleFinder-0.1.3/tests/test_6_stec_aa_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2022-03-21 20:37:30.000000 AlleleFinder-0.1.3/tests/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2829 2023-02-28 19:59:56.000000 AlleleFinder-0.1.3/tests/test_0_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3249 2023-06-19 15:57:17.000000 AlleleFinder-0.1.3/tests/test_7_stec_allele_split.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4265 2023-06-19 15:58:02.000000 AlleleFinder-0.1.3/tests/test_8_stec_allele_concatenate.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     7795 2023-06-01 15:06:39.000000 AlleleFinder-0.1.3/tests/test_2_allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3042 2023-03-13 19:11:01.000000 AlleleFinder-0.1.3/tests/test_4_stec_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/setup.cfg
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/
+-rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)     1113 2023-02-24 20:49:53.000000 AlleleFinder-0.1.4/setup.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1077 2023-03-10 15:09:59.000000 AlleleFinder-0.1.4/LICENSE
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/PKG-INFO
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/AlleleFinder.egg-info/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      742 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/AlleleFinder.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       19 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/AlleleFinder.egg-info/top_level.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/AlleleFinder.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/AlleleFinder.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     9315 2023-06-21 02:14:21.000000 AlleleFinder-0.1.4/README.md
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/allele_tools/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    24429 2023-03-24 14:27:36.000000 AlleleFinder-0.1.4/allele_tools/allele_profiler.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35689 2023-06-21 18:08:55.000000 AlleleFinder-0.1.4/allele_tools/stec.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-06-22 16:34:50.000000 AlleleFinder-0.1.4/allele_tools/__init__.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6600 2023-07-05 14:06:55.000000 AlleleFinder-0.1.4/allele_tools/profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    98410 2023-06-29 18:55:47.000000 AlleleFinder-0.1.4/allele_tools/methods.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       51 2023-07-13 15:12:40.000000 AlleleFinder-0.1.4/allele_tools/version.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    28340 2023-03-24 18:52:09.000000 AlleleFinder-0.1.4/allele_tools/allele_updater.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35343 2023-03-24 19:36:21.000000 AlleleFinder-0.1.4/allele_tools/allele_translate_reduce.py
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/tests/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4680 2023-06-19 16:07:38.000000 AlleleFinder-0.1.4/tests/test_5_stec_allele_find.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6584 2023-06-01 15:06:40.000000 AlleleFinder-0.1.4/tests/test_1_allele_translate_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4628 2023-03-13 20:02:00.000000 AlleleFinder-0.1.4/tests/test_3_stec_profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2107 2023-06-19 16:16:44.000000 AlleleFinder-0.1.4/tests/test_6_stec_aa_allele_find.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2022-03-21 20:37:30.000000 AlleleFinder-0.1.4/tests/__init__.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2829 2023-02-28 19:59:56.000000 AlleleFinder-0.1.4/tests/test_0_profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3249 2023-06-19 15:57:17.000000 AlleleFinder-0.1.4/tests/test_7_stec_allele_split.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4265 2023-06-19 15:58:02.000000 AlleleFinder-0.1.4/tests/test_8_stec_allele_concatenate.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     7795 2023-06-01 15:06:39.000000 AlleleFinder-0.1.4/tests/test_2_allele_updater.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3042 2023-03-13 19:11:01.000000 AlleleFinder-0.1.4/tests/test_4_stec_allele_translate_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2023-07-19 14:35:17.000000 AlleleFinder-0.1.4/setup.cfg
```

### Comparing `AlleleFinder-0.1.3/setup.py` & `AlleleFinder-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/LICENSE` & `AlleleFinder-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/AlleleFinder.egg-info/SOURCES.txt` & `AlleleFinder-0.1.4/AlleleFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/README.md` & `AlleleFinder-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](https://OLC-Bioinformatics.github.io/AlleleFinder/?badge=stable)
 [![license](https://img.shields.io/badge/license-MIT-brightgreen)](https://github.com/OLC-Bioinformatics/AlleleFinder/blob/main/LICENSE)
 
 
 
 ### STEC AlleleFinder
 
-A suite of tools, written in Python, designed for the discovery, sequence typing, and profiling the _stx_ alleles in Shiga toxin-producing _E. coli_  
+A suite of tools, written in Python, designed for the discovery, sequence typing, and profiling the _stx_ alleles in Shiga toxin-producing _Escherichia coli_  
 
 ## Scripts
 
-There is a single STEC script with five separate functionalities:
+There is a single STEC script with six separate functionalities:
 
 1. [`profile_reduce`](https://olc-bioinformatics.github.io/AlleleFinder/profile_reduce)
 2. [`allele_translate_reduce`](https://olc-bioinformatics.github.io/AlleleFinder/allele_translate_reduce)
 3. [`allele_find`](https://olc-bioinformatics.github.io/AlleleFinder/allele_find)
 4. [`aa_allele_find`](https://olc-bioinformatics.github.io/AlleleFinder/aa_allele_find)
 5. [`allele_split`](https://olc-bioinformatics.github.io/AlleleFinder/allele_split)
+6. [`allele_concatenate`](https://olc-bioinformatics.github.io/AlleleFinder/allele_concatenate)
 
 
 Full documentation is available at the [AlleleFinder GitHub pages site](https://olc-bioinformatics.github.io/AlleleFinder/)
 
 ## Quick Start
 
 [`Conda`](https://docs.conda.io/en/latest/) is required to install AlleleFinder. See the [documentation](http://bioconda.github.io/) or [AlleleFinder installation](https://olc-bioinformatics.github.io/AlleleFinder/install/) for instructions of getting conda installed on your system
@@ -156,14 +157,27 @@
 ```
 stec.py allele_split -q /path/to/query_folder -o /path/to_output_folder
 ```
 
 Additional information regarding this functionality is available in the [`allele_split`](https://olc-bioinformatics.github.io/AlleleFinder/allele_split) documentation
 
 
+## Concatenate allele database
+
+This script concatenates alleles of the _stx_ A and B subunits into a single sequence with a linker
+
+1. nucleotide and amino acid allele files prepare by [`allele_translate_reduce`](https://olc-bioinformatics.github.io/AlleleFinder/allele_translate_reduce)
+2. nucleotide and amino acid profile files prepared by [`allele_translate_reduce`](https://olc-bioinformatics.github.io/AlleleFinder/allele_translate_reduce). Note that the allele files must contain sequence for the same genes that were used for the reduction of the profile, e.g.:
+
+#### Running the script
+
+```
+stec.py allele_concatenate --nt_profile /path/to/nt_profile/profile.txt --aa_profile /path/to/aa_profile/profile.txt --nt_alleles /path/to/nt_alleles --aa_alleles /path/to/aa_alleles -c /path/to/outputs
+```
+
 ## Feedback
 
 If you encounter any issues installing or running AlleleFinder, have feature requests, or need assistance, please [open an issue on GitHub](https://github.com/OLC-Bioinformatics/AlleleFinder/issues/new/choose)
 
 
 ## License
```

### Comparing `AlleleFinder-0.1.3/allele_tools/allele_profiler.py` & `AlleleFinder-0.1.4/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/allele_tools/stec.py` & `AlleleFinder-0.1.4/allele_tools/stec.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,15 @@
             allele_path=self.nt_allele_path,
             allele_order=self.allele_order
         )
         self.gene, self.aa_alleles = load_alleles(
             allele_path=self.aa_allele_path,
             allele_order=self.allele_order
         )
+        logging.info('Concatenating allele sequences')
         self.concatenated_nt_seq = concatenate_alleles(
             profile_data=self.nt_profile_data,
             allele_dict=self.nt_alleles,
             allele_order=self.allele_order,
             stx_gene=self.gene,
             linker_length_dict=self.linker_length_dict,
             molecule='nt'
@@ -372,14 +373,15 @@
             profile_data=self.aa_profile_data,
             allele_dict=self.aa_alleles,
             allele_order=self.allele_order,
             stx_gene=self.gene,
             linker_length_dict=self.linker_length_dict,
             molecule='aa'
         )
+        logging.info('Writing concatenated allele sequences to file')
         write_concatenated_sequences(
             concatenated_sequences=self.concatenated_nt_seq,
             concatenate_path=self.concatenate_path,
             file_name=self.gene_allele[self.gene],
             molecule='nt'
         )
         write_concatenated_sequences(
```

### Comparing `AlleleFinder-0.1.3/allele_tools/profile_reduce.py` & `AlleleFinder-0.1.4/allele_tools/profile_reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,19 @@
                         # Extract the sequence type from the 'ST' column
                         seq_type = allele_dict['ST']
                         # Initialise variables to store the allele numbering information
                         allele_list = []
                         allele_str = ''
                         # Iterate through all the genes of interest
                         for gene in self.names:
-                            allele_str += allele_dict[gene]
+                            try:
+                                allele_str += allele_dict[gene]
+                            # If an allele has been filtered based on length, the sequence type needs to be removed
+                            except TypeError:
+                                continue
                             # Add the allele number to the list, and to the string
                             allele_list.append(allele_dict[gene])
                         # Check if the string of allele numbers is already in the dictionary
                         if allele_str not in profile_st:
                             # Update the dictionary with the string of alleles: sequence type
                             profile_st[allele_str] = allele_dict[self.names[0]]
                             alleles = '\t'.join(allele_list)
@@ -92,15 +96,15 @@
 
     def __init__(self, profile, names, output='profile'):
         logging.info('Welcome to profile reducer!')
         self.profile = pathfinder(path=profile)
         try:
             assert os.path.isfile(self.profile)
         except AssertionError as exc:
-            logging.error('Cannot locate the specified profile file: %s, (self.profile,)')
+            logging.error('Cannot locate the specified profile file: %s', self.profile)
             raise SystemExit from exc
         # Create the folder into which the reduced profile and notes are to be placed
         self.report_path = os.path.join(os.path.dirname(self.profile), output)
         make_path(self.report_path)
         self.reduced_profile = os.path.join(self.report_path, 'profile.txt')
         self.notes_file = os.path.join(self.report_path, 'reducing_notes.txt')
         self.name_file = pathfinder(path=names)
@@ -130,16 +134,18 @@
         metavar='names',
         required=True,
         help='Name and path to a file containing the gene names (one per line) to be extracted '
              'from the profile')
     # Get the arguments into an object
     arguments = parser.parse_args()
     SetupLogging(debug=True)
-    reduce = ProfileReduce(profile=arguments.profile,
-                           names=arguments.names)
+    reduce = ProfileReduce(
+        profile=arguments.profile,
+        names=arguments.names
+    )
     reduce.main()
     logging.info('Profile reduction complete!')
     # Prevent the arguments being printed to the console (they are returned in order for the tests to work)
     sys.stderr = open(os.devnull, 'w', encoding='utf-8')
     return arguments
```

### Comparing `AlleleFinder-0.1.3/allele_tools/methods.py` & `AlleleFinder-0.1.4/allele_tools/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,19 +1071,31 @@
                     # contig:query_range combination
                     else:
                         # Iterate over each gene in the gene_pair tuple
                         for i, gene_name in enumerate(gene_pair):
                             # Extract the gene_alleleID from the dictionary for this gene
                             corresponding_allele = info_dict['allele'][i]
                             # Remove the gene name information from the corresponding_allele variable
-                            allele_number = corresponding_allele.replace(f'{gene_name}_', '')
-                            # Update the dictionary with the new gene: allele number for the sample
-                            allele_comprehension[contig][query_range].update(
-                                {gene_name: allele_number}
-                            )
+
+                            if gene_name in corresponding_allele:
+                                allele_number = corresponding_allele.replace(f'{gene_name}_', '')
+                                # Update the dictionary with the new gene: allele number for the sample
+                                allele_comprehension[contig][query_range].update(
+                                    {gene_name: allele_number}
+                                )
+                            else:
+                                # Determine which gene(s) are not currently being examined
+                                corresponding_gene = [
+                                    other_gene for other_gene in gene_names if other_gene != gene_name
+                                ][0]
+                                allele_number = corresponding_allele.replace(f'{corresponding_gene}_', '')
+                                # Update the dictionary with the new gene: allele number for the sample
+                                allele_comprehension[contig][query_range].update(
+                                    {corresponding_gene: allele_number}
+                                )
         # If the allele_comprehension dictionary exists, it doesn't need to be further populated
         if allele_comprehension:
             continue
         # Otherwise iterate through the targetsequence dictionary
         for contig, range_dict in sample.alleles.targetsequence.items():
             # Update the allele comprehension dictionary as required
             if contig not in allele_comprehension:
@@ -1534,16 +1546,22 @@
     seq_type_str = f'{next_seq_type}'
     # Initialise a header to store 'ST  gene1   gene2.......geneX\n'
     header = 'ST'
     # Iterate over all the genes in the analysis
     for gene in genes:
         # Extract the allele ID for each gene in the analysis
         allele = allele_dict[gene]
+        # If the allele has been filtered return False, as a sequence type should not exist for filtered alleles
         if not allele:
             return False
+        # Check if the gene name is in the allele
+        if gene in allele:
+            # Extract the allele number
+            allele = allele.split('_')[-1]
+
         # Update the header with the gene
         header += f'\t{gene}'
         # Update the profile string with the allele ID
         seq_type_str += f'\t{allele}'
     # Open the profile file (to update) and write the novel profile
     with open(profile_file, 'a+', encoding='utf-8') as profile:
         profile.write(seq_type_str + '\n')
@@ -1978,14 +1996,16 @@
     concatenated_sequences = []
     # Iterate over all the sequence type: profile pairs in profile_data
     for seq_type, profile in profile_data.items():
         # Initialise a string to store the concatenated sequences
         concatenated_seq = str()
         # Create a boolean to store if one (or both) of the allele subunits is missing
         complete = True
+        # Create a variable to store the name of the concatenated allele
+        concatenated_name = str()
         # Iterate over the subunits in order from the allele_order dictionary
         for subunit in allele_order[stx_gene]:
             # Extract the allele number from the profile dictionary using the subunit as the key
             allele_number = profile[subunit]
             # If the allele number is 0, the subunit is absent, and the concatenated sequence will not be created
             if allele_number == '0':
                 complete = False
@@ -2004,22 +2024,27 @@
                 # Nucleotide sequences will use N as the linker sequence
                 if molecule == 'nt':
                     linker = 'N' * linker_length
                 # Amino acid sequences will use X as the linker sequence, and will be reduced by a factor of three
                 else:
                     linker = 'X' * int(linker_length / 3)
                 concatenated_seq += f'{allele_seq}{linker}'
+            # Update the name of the concatenated sequence
+            if concatenated_name:
+                concatenated_name += f'_{allele_number}'
+            else:
+                concatenated_name = allele_number
         # Do not add incomplete sequences to the list
         if not complete:
             continue
         # Create a SeqRecord of the allele using the novel allele name and sequence
         concatenated_sequences.append(
             SeqRecord(
                 seq=Seq(concatenated_seq),
-                id=seq_type,
+                id=concatenated_name,
                 name='',
                 description=''
             )
         )
     return concatenated_sequences
```

### Comparing `AlleleFinder-0.1.3/allele_tools/allele_updater.py` & `AlleleFinder-0.1.4/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/allele_tools/allele_translate_reduce.py` & `AlleleFinder-0.1.4/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_5_stec_allele_find.py` & `AlleleFinder-0.1.4/tests/test_5_stec_allele_find.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_1_allele_translate_reduce.py` & `AlleleFinder-0.1.4/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_3_stec_profile_reduce.py` & `AlleleFinder-0.1.4/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_6_stec_aa_allele_find.py` & `AlleleFinder-0.1.4/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_0_profile_reduce.py` & `AlleleFinder-0.1.4/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_7_stec_allele_split.py` & `AlleleFinder-0.1.4/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_8_stec_allele_concatenate.py` & `AlleleFinder-0.1.4/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_2_allele_updater.py` & `AlleleFinder-0.1.4/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.3/tests/test_4_stec_allele_translate_reduce.py` & `AlleleFinder-0.1.4/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

