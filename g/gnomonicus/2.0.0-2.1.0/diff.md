# Comparing `tmp/gnomonicus-2.0.0.tar.gz` & `tmp/gnomonicus-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnomonicus-2.0.0.tar", last modified: Fri Jun 30 10:10:09 2023, max compression
+gzip compressed data, was "gnomonicus-2.1.0.tar", last modified: Wed Jul 19 11:43:30 2023, max compression
```

## Comparing `gnomonicus-2.0.0.tar` & `gnomonicus-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.289426 gnomonicus-2.0.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/bin/gbkToPkl
--rwxr-xr-x   0 runner    (1001) docker     (123)     8844 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/bin/gnomonicus
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.289426 gnomonicus-2.0.0/gnomonicus/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/gnomonicus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/gnomonicus/gnomonicus_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/gnomonicus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:09:20.000000 gnomonicus-2.0.0/gnomonicus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:43:30.912189 gnomonicus-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-19 11:42:44.000000 gnomonicus-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-19 11:43:30.912189 gnomonicus-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-19 11:42:44.000000 gnomonicus-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:43:30.912189 gnomonicus-2.1.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-19 11:42:44.000000 gnomonicus-2.1.0/bin/gbkToPkl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9098 2023-07-19 11:42:44.000000 gnomonicus-2.1.0/bin/gnomonicus
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:43:30.912189 gnomonicus-2.1.0/gnomonicus/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-19 11:42:44.000000 gnomonicus-2.1.0/gnomonicus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48039 2023-07-19 11:42:44.000000 gnomonicus-2.1.0/gnomonicus/gnomonicus_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:43:30.912189 gnomonicus-2.1.0/gnomonicus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-19 11:43:30.000000 gnomonicus-2.1.0/gnomonicus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-19 11:43:30.000000 gnomonicus-2.1.0/gnomonicus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:43:30.000000 gnomonicus-2.1.0/gnomonicus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:42:51.000000 gnomonicus-2.1.0/gnomonicus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 11:43:30.000000 gnomonicus-2.1.0/gnomonicus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 11:43:30.000000 gnomonicus-2.1.0/gnomonicus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-19 11:42:44.000000 gnomonicus-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-19 11:43:30.916189 gnomonicus-2.1.0/setup.cfg
```

### Comparing `gnomonicus-2.0.0/LICENSE` & `gnomonicus-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.0.0/PKG-INFO` & `gnomonicus-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomonicus
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 Home-page: https://github.com/oxfordmmm/gnomonicus
 Author: Philip W Fowler, Jeremy Westhead
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford License, see LICENSE
 Keywords: gnomonicus,piezo,lodestone,clockwork,TB
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gnomonicus-2.0.0/README.md` & `gnomonicus-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.0.0/bin/gbkToPkl` & `gnomonicus-2.1.0/bin/gbkToPkl`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.0.0/bin/gnomonicus` & `gnomonicus-2.1.0/bin/gnomonicus`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     parser.add_argument("--progress",action='store_true',default=False,help="whether to show progress using tqdm")
     parser.add_argument("--output_dir", required=False, default=".", help="Directory to save output files to. Defaults to wherever the script is run from.")
     parser.add_argument("--json", required=False, action='store_true', default=False, help="Flag to create a single JSON output as well as the CSVs")
     parser.add_argument("--fasta", required=False, default=None, help="Use to output a FASTA file of the resultant genome. Specify either 'fixed' or 'variable' for fixed length and variable length FASTA respectively. Alternatively, use 'both' to produce both")
     parser.add_argument("--minor_populations", required=False, default=None, help="Path to a line separated file containing genome indices of minor populations.")
     parser.add_argument("--csvs", required=False, nargs="+", help="Types of CSV to produce. Accepted values are [variants, mutations, effects, predictions, all]. `all` produces all of the CSVs")
     parser.add_argument("--debug", default=False, action='store_true', help='Whether to log debugging messages to the log. Defaults to False')
+    parser.add_argument("--resistance_genes", required=False, default=False, action="store_true", help="Flag to filter mutations and variants to only include genes present in the resistance catalogue")
     options = parser.parse_args()
 
     options.output_dir = os.path.realpath(options.output_dir)
 
     #Make the output directory if it doesn't already exist
     os.makedirs(options.output_dir, exist_ok=True)
 
@@ -111,19 +112,19 @@
 
     #Complain if there are no variants
     if diff.variants is None:
         logging.error("No variants detected!")
         raise Exception("No variants detected!")
 
     #Get the variations and mutations
-    variants = populateVariants(vcfStem, options.output_dir, diff, make_variants_csv, catalogue=resistanceCatalogue)
+    variants = populateVariants(vcfStem, options.output_dir, diff, make_variants_csv, options.resistance_genes, catalogue=resistanceCatalogue)
     logging.debug("Populated and saved variants.csv")
 
     mutations, referenceGenes = populateMutations(vcfStem, options.output_dir, diff, 
-                        reference, sample, resistanceCatalogue, make_mutations_csv)
+                        reference, sample, resistanceCatalogue, make_mutations_csv, options.resistance_genes)
     if mutations is None:
         logging.info("No mutations found - probably due to exclusively inter-gene variation or no variation.\n\t\t\t\t\t\t\t No effects.csv written")
     else:
         logging.debug("Populated and saved mutatons.csv")
 
     #Get the effects of the mutations
     if resistanceCatalogue is not None and mutations is not None:
```

### Comparing `gnomonicus-2.0.0/gnomonicus/__init__.py` & `gnomonicus-2.1.0/gnomonicus/__init__.py`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.0.0/gnomonicus/gnomonicus_lib.py` & `gnomonicus-2.1.0/gnomonicus/gnomonicus_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,22 @@
         Args:
             gene (str): Name of the gene
             mutation (str): The invalid mutation
         '''
         self.message = f"{gene}@{mutation} is not a valid mutation!"
         super().__init__(self.message)
 
+class OutdatedGumpyException(Exception):
+    '''Custom exception raised if a pickled gumpy.Genome object doesn't match
+    the version currently being used here. 
+    '''
+    def __init__(self):
+        self.message = "This Genome object is outdated! Pass a genbank file to re-instanciate"
+        super().__init__(self.message)
+
 def checkGzip(path: str) -> bool:
     '''Check if a given path is a gzipped file
 
     Args:
         path (str): Path to the file
 
     Returns:
@@ -66,46 +74,79 @@
     #Remove trailing '/' if required
     if path[-1] == '/':
         path = path[:-1]
 
     #Check if the file is gzipped
     gzipped = checkGzip(path)
 
+    #Get the gumpy version we are using
+    gumpy_major, gumpy_minor, gumpy_maintainance = gumpy.__version__[1:].split(".")
+    outdated = False
+
     #Try to load as a pickle
     try:
         if gzipped:
             logging.info("Path was to a gzipped file. Decompressing...")
             f = gzip.open(path, 'rb')
         else:
             logging.info("Path was not to a gzipped file. Defaulting to normal reading")
             f = open(path, 'rb')
-        return pickle.load(f)
+        g = pickle.load(f)
+        if hasattr(g, 'gumpy_version'):
+            #Has the version set, so check it
+            major, minor, maintainance = g.gumpy_version[1:].split(".")
+            if major == gumpy_major and minor == gumpy_minor and maintainance == gumpy_maintainance:
+                #Exact match to the gumpy version
+                return g
+            else:
+                outdated = True
+        else:
+            outdated = True
+        if outdated:
+            logging.error("Genome object is outdated!")
+            raise OutdatedGumpyException()
+    except OutdatedGumpyException as e:
+        logging.error("Genome object is outdated!")
+        raise e
     except Exception as e:
         logging.info(f"Genome object not a pickle, checking if pickled version exists. Error: {e}")
 
     #Try pickled version created by this (path+'.pkl')
     #Check if this file is gzipped
     gzipped = checkGzip(path+".pkl")
     try:
         if gzipped:
             logging.info("Path was to a gzipped file. Decompressing...")
             f = gzip.open(path+".pkl", 'rb')
         else:
             logging.info("Path was not to a gzipped file. Defaulting to normal reading")
             f = open(path+".pkl", 'rb')
-        return pickle.load(f)
+        g = pickle.load(f)
+        if hasattr(g, 'gumpy_version'):
+            #Has the version set, so check it
+            major, minor, maintainance = g.gumpy_version[1:].split(".")
+            if major == gumpy_major and minor == gumpy_minor and maintainance == gumpy_maintainance:
+                #Exact match to the gumpy version
+                return g
+            else:
+                outdated = True
+        else:
+            outdated = True
+        if outdated:
+            logging.info("Genome object is outdated! Trying with the original filepath")
     except Exception as e:
         logging.info(f"No pickled version of genome object, instanciating and dumping. Error: {e}")
     
     #Create new gumpy.Genome and pickle dump for speed later
     reference = gumpy.Genome(path, show_progress_bar=progress)
+    reference.gumpy_version = gumpy.__version__
     pickle.dump(reference, open(path+'.pkl', 'wb'))
     return reference
 
-def populateVariants(vcfStem: str, outputDir: str, diff: gumpy.GenomeDifference, make_csv: bool, catalogue: piezo.ResistanceCatalogue=None) -> pd.DataFrame:
+def populateVariants(vcfStem: str, outputDir: str, diff: gumpy.GenomeDifference, make_csv: bool, resistanceGenesOnly: bool, catalogue: piezo.ResistanceCatalogue=None) -> pd.DataFrame:
     '''Populate and save the variants DataFrame as a CSV
 
     Args:
         vcfStem (str): The stem of the filename for the VCF file. Used as a uniqueID
         outputDir (str): Path to the desired output directory
         diff (gumpy.GenomeDifference): GenomeDifference object between reference and the sample
         make_csv (bool): Whether to write the CSV of the dataframe
@@ -122,17 +163,42 @@
             'indel_nucleotides': diff.indel_nucleotides,
             'vcf_evidence': [json.dumps(x) for x in diff.vcf_evidences],
             'vcf_idx': diff.vcf_idx,
             'gene_name': diff.gene_name,
             'gene_position': diff.gene_pos,
             'codon_idx': diff.codon_idx
             }
-    variants = pd.DataFrame(vals)
+
+    #Use of Int64 rather than int is required here as pandas doesn't allow mixed int/None
+    variants = pd.DataFrame(vals).astype(
+        {
+            'vcf_evidence': 'object',
+            'nucleotide_index': 'Int64',
+            'indel_length': 'Int64',
+            'vcf_idx': 'Int64',
+            'gene_position': 'Int64',
+            'codon_idx': 'Int64'
+        }
+    )
+
+    if catalogue is not None:
+        #Figure out if we want to keep all of the variants
+        genes = getGenes(diff, catalogue, resistanceGenesOnly)
+        to_drop = []
+        for idx, row in variants.iterrows():
+            if row['gene_name'] not in genes:
+                #Not a variant we're interested in, so remove
+                to_drop.append(idx)
+                
+        variants.drop(index=to_drop, inplace=True)
+    else:
+        genes = set(diff.genome2.genes.keys())
+
     if diff.genome1.minor_populations or diff.genome2.minor_populations:
-        variants = pd.concat([variants, minority_population_variants(diff, catalogue)])
+        variants = pd.concat([variants, minority_population_variants(diff, catalogue, genes)])
 
     #If there are variants, save them to a csv
     if not variants.empty:
         #Add unique ID to each record
         variants['uniqueid'] = vcfStem
 
         variants = variants[['uniqueid', 'variant', 'gene_name', 'gene_position', 'codon_idx', 'nucleotide_index', 'indel_length', 'indel_nucleotides', 'vcf_evidence', 'vcf_idx']]
@@ -170,37 +236,34 @@
                     cov += 1
     #We have just COV
     if cov > 0 and frs == 0:
         return 'reads'
     #We have anything else
     return 'percentage'
 
-def populateMutations(
-        vcfStem: str, outputDir: str, diff: gumpy.GenomeDifference, reference: gumpy.Genome,
-        sample: gumpy.Genome, resistanceCatalogue: piezo.ResistanceCatalogue, make_csv: bool) -> (pd.DataFrame, dict):
-    '''Popuate and save the mutations DataFrame as a CSV, then return it for use in predictions
+def getGenes(diff: gumpy.GenomeDifference, resistanceCatalogue: piezo.ResistanceCatalogue, resistanceGenesOnly: bool) -> set:
+    '''Get the genes we're interested in. 
+    
+    This is either just resistance genes which have variants, or all which have variants
 
     Args:
-        vcfStem (str): The stem of the filename of the VCF file. Used as a uniqueID
-        outputDir (str): Path to the desired output directory
-        diff (gumpy.GenomeDifference): GenomeDifference object between reference and this sample
-        reference (gumpy.Genome): Reference genome
-        sample (gumpy.Genome): Sample genome
-        resistanceCatalogue (piezo.ResistanceCatalogue): Resistance catalogue (used to find which genes to check)
-        make_csv (bool): Whether to write the CSV of the dataframe
-
-    Raises:
-        MissingFieldException: Raised when the mutations DataFrame does not contain the required fields
+        diff (gumpy.GenomeDifference): Genome Difference between reference and sample
+        resistanceCatalogue (piezo.ResistanceCatalogue): Resistance catalogue
+        resistanceGenesOnly (bool): Whether to just use genes within the catalogue
 
     Returns:
-        pd.DataFrame: The mutations DataFrame
-        dict: Dictionary mapping gene name --> reference gumpy.Gene object
+        set[str]: Set of gene names
     '''
-    #For the sake of consistency, moving towards including all genes with mutations (not just those in the catalogue)
+    reference = diff.genome1
+    sample = diff.genome2
     if resistanceCatalogue:
+        if resistanceGenesOnly:
+            resistanceGenes = set(resistanceCatalogue.catalogue.genes)
+        else:
+            resistanceGenes = set(sample.genes)
         #Find the genes which have mutations regardless of being in the catalogue
         #Still cuts back time considerably, and ensures all mutations are included in outputs
         mask = np.isin(reference.stacked_nucleotide_index, diff.nucleotide_index)
         genesWithMutations = np.unique(reference.stacked_gene_name[mask]).tolist()
 
         #Make sure minority population mutations are also picked up
         minor_genes = set()
@@ -212,17 +275,43 @@
 
         deletions = []
         #Make sure large deletions are picked up too
         for name in reference.stacked_gene_name:
             deletions += np.unique(name[sample.is_deleted]).tolist()
         genesWithMutations = set(genesWithMutations + deletions)
 
+        return genesWithMutations.intersection(resistanceGenes)
+
     else:
         #No catalogue, so just stick to genes in the sample
-        genesWithMutations = sample.genes
+        return sample.genes
+
+def populateMutations(
+        vcfStem: str, outputDir: str, diff: gumpy.GenomeDifference, reference: gumpy.Genome,
+        sample: gumpy.Genome, resistanceCatalogue: piezo.ResistanceCatalogue, make_csv: bool, resistanceGenesOnly: bool) -> (pd.DataFrame, dict):
+    '''Popuate and save the mutations DataFrame as a CSV, then return it for use in predictions
+
+    Args:
+        vcfStem (str): The stem of the filename of the VCF file. Used as a uniqueID
+        outputDir (str): Path to the desired output directory
+        diff (gumpy.GenomeDifference): GenomeDifference object between reference and this sample
+        reference (gumpy.Genome): Reference genome
+        sample (gumpy.Genome): Sample genome
+        resistanceCatalogue (piezo.ResistanceCatalogue): Resistance catalogue (used to find which genes to check)
+        make_csv (bool): Whether to write the CSV of the dataframe
+        resistanceGenesOnly (bool): Whether to use just genes present in the resistance catalogue
+
+    Raises:
+        MissingFieldException: Raised when the mutations DataFrame does not contain the required fields
+
+    Returns:
+        pd.DataFrame: The mutations DataFrame
+        dict: Dictionary mapping gene name --> reference gumpy.Gene object
+    '''
+    genesWithMutations = getGenes(diff, resistanceCatalogue, resistanceGenesOnly)
 
     #Iter resistance genes with variation to produce gene level mutations - concating into a single dataframe
     mutations = None
     referenceGenes = {}
     diffs = []
     #This is where the majority of the time to process is used.
     #However, I have tried a few ways to improve this involving reducing reliance on DF concat
@@ -278,23 +367,23 @@
                     mutations = pd.concat([mutations, geneMutations])
                 else:
                     mutations = geneMutations
     if mutations is not None:
         #Ensure correct datatypes
         mutations = mutations.astype({'mutation': 'str',
                                     'gene': 'str',
-                                    'nucleotide_number': 'float',
-                                    'nucleotide_index': 'float',
-                                    'gene_position': 'float',
+                                    'nucleotide_number': 'Int64',
+                                    'nucleotide_index': 'Int64',
+                                    'gene_position': 'Int64',
                                     'alt': 'str',
                                     'ref': 'str',
                                     'codes_protein': 'bool',
-                                    'indel_length': 'float',
+                                    'indel_length': 'Int64',
                                     'indel_nucleotides': 'str',
-                                    'amino_acid_number': 'float',
+                                    'amino_acid_number': 'Int64',
                                     'amino_acid_sequence': 'str',
                                 })
     #Add minor mutations (these are stored separately)
     if reference.minor_populations or sample.minor_populations:
         #Only do this if they exist
         x = minority_population_mutations(diffs, resistanceCatalogue)
         mutations = pd.concat([mutations, x])
@@ -324,20 +413,21 @@
                         to_drop.append(idx)
             mutations_.drop(index=to_drop, inplace=True)
             #Save it as CSV
             mutations_.to_csv(os.path.join(outputDir, f'{vcfStem}.mutations.csv'), index=False)
 
     return mutations, referenceGenes
 
-def minority_population_variants(diff: gumpy.GenomeDifference, catalogue: piezo.ResistanceCatalogue) -> pd.DataFrame:
+def minority_population_variants(diff: gumpy.GenomeDifference, catalogue: piezo.ResistanceCatalogue, genes: set) -> pd.DataFrame:
     '''Handle the logic for pulling out minority population calls for genome level variants
 
     Args:
         diff: (gumpy.GenomeDifference): GenomeDifference object for this comparison
         catalogue: (piezo.ResistanceCatalogue): Catalogue to use. Used for determining whether FRS or COV should be used
+        genes (set[str]): Set of gene names we care about
 
     Returns:
         pd.DataFrame: DataFrame containing the minority population data
     '''
     #Determine if FRS or COV should be used
     minor_type = get_minority_population_type(catalogue)
 
@@ -350,20 +440,36 @@
     vcf_evidences = []
     vcf_idx = []
     gene_name = []
     gene_pos = []
     codon_idx = []
     variants = []
 
+    if genes is not None:
+        #Using the gene names, find out which genome indices we want to look out for
+        indices_we_care_about = []
+        for gene in genes:
+            mask = diff.genome1.stacked_gene_name == gene
+            gene_indices = diff.genome1.stacked_nucleotide_index[mask].tolist()
+            indices_we_care_about += gene_indices
+        indices_we_care_about = set(indices_we_care_about)
+    else:
+        #Genes was none, so fetch everything
+        indices_we_care_about = set(diff.genome1.nucleotide_index)
+
+
     for variant_ in variants_:
         variant, evidence = variant_.split(":")
         variants.append(variant_)
         
         if ">" in variant:
             idx = int(variant.split(">")[0][:-1])
+            if idx not in indices_we_care_about:
+                variants.pop()
+                continue
             nucleotide_indices.append(idx)
             vcf = diff.genome2.vcf_evidence.get(int(variant.split(">")[0][:-1]))
             vcf_evidences.append(json.dumps(vcf))
             
             ref = variant.split(">")[0][-1]
             alt = variant.split(">")[-1]
 
@@ -371,15 +477,16 @@
                 #Wildtype call so return 0 as it isn't an ALT
                 vcf_idx.append(0)
             else:
                 #Simple SNP so check for presence in alts + right COV
                 ev = float(evidence)
                 if ev < 1:
                     #We have FRS so (due to rounding) convert the VCF's COV to FRS
-                    cov = [round(x/vcf['DP'], 3) for x in vcf["COV"]]
+                    total_depth = sum(vcf['COV'])
+                    cov = [round(x/total_depth, 3) for x in vcf["COV"]]
                 else:
                     cov = vcf['COV']
                 minor_call = variant.split(">")[-1]
 
                 added = False
                 for v_idx, alt in enumerate(vcf['ALTS']):
                     v_idx += 1
@@ -398,23 +505,27 @@
                 #Shouldn't be possible, but check anyway
                 assert added, f"The index of the VCF evidence could not be determined! {variant_} --> {vcf}"                        
 
 
 
         else:
             idx = int(variant.split("_")[0])
+            if idx not in indices_we_care_about:
+                variants.pop()
+                continue
             nucleotide_indices.append(idx)
             vcf = diff.genome2.vcf_evidence.get(int(variant.split("_")[0]))
             vcf_evidences.append(json.dumps(vcf))
 
             #Match VCF idx on base changes + cov
             ev = float(evidence)
             if ev < 1:
                 #We have FRS so (due to rounding) convert the VCF's COV to FRS
-                cov = [round(x/vcf['DP'], 3) for x in vcf["COV"]]
+                total_depth = sum(vcf['COV'])
+                cov = [round(x/total_depth, 3) for x in vcf["COV"]]
             else:
                 cov = vcf['COV']
             
             ref = vcf['REF']
             type_ = variant.split("_")[1]
             bases = variant.split("_")[-1]
             added = False
@@ -503,15 +614,20 @@
         'gene_name': gene_name,
         'gene_position': gene_pos,
         'codon_idx': codon_idx
         }
     #Convert everything to numpy arrays
     vals = {key: np.array(vals[key]) for key in vals.keys()}
     return pd.DataFrame(vals).astype({
-                                    'vcf_evidence': 'object'
+                                    'vcf_evidence': 'object',
+                                    'nucleotide_index': 'Int64',
+                                    'indel_length': 'Int64',
+                                    'vcf_idx': 'Int64',
+                                    'gene_position': 'Int64',
+                                    'codon_idx': 'Int64'
                                 })
 
 
 def minority_population_mutations(diffs: [gumpy.GeneDifference], catalogue: piezo.ResistanceCatalogue) -> pd.DataFrame:
     '''Handle the logic for pulling out minority population calls for gene level variants
 
     Args:
@@ -571,22 +687,28 @@
             is_null.append("X" in mut.upper())
             is_promoter.append(num < 0)
             variants.append(None)
             number_nucleotide_changes.append(diff.gene2.minor_nc_changes[num])
 
             if "_" in mut:
                 #Indel
-                _, t, bases = mut.split("_")
+                if len(mut.split("_")) == 3:
+                    _, t, bases = mut.split("_")
+                    indel_nucleotides.append(bases)
+                    if t == "del":
+                        indel_length.append(-1 * len(bases))
+                    else:
+                        indel_length.append(len(bases))              
+                else:
+                    #We have a `<pos>_indel` or `<pos>_mixed`
+                    indel_nucleotides.append(None)
+                    indel_length.append(None)
                 ref.append(None)
                 alt.append(None)
-                if t == "del":
-                    indel_length.append(-1 * len(bases))
-                else:
-                    indel_length.append(len(bases))
-                indel_nucleotides.append(bases)
+
                 is_snp.append(False)
                 nucleotide_number.append(num)
                 nucleotide_index.append(diff.gene1.nucleotide_index[diff.gene1.nucleotide_number == num][0])
                 aa_num.append(None)
                 aa_seq.append(None)
                 continue
             else:
@@ -692,15 +814,15 @@
                 #Is a nucleotide (non-promoter) mutation in a coding gene
                 #So skip it as it may cause prediction problems
                 continue
         #Remove large dels if not supported
         if not large_dels:
             #Check if this is a large del
             large = re.compile(r"""
-                                del_(1\.0)|(0\.[0-9][0-9])
+                                del_(1\.0)|(0\.[0-9][0-9]?[0-9]?)
                                 """, re.VERBOSE)
             if large.fullmatch(mutation):
                 continue
         fixed.append((gene, mutation))
     return fixed
 
 def populateEffects(
@@ -895,50 +1017,50 @@
         meta['catalogue_name'] = None
         meta['catalogue_version'] = None
     data = {}
     #Variants field
     _variants = []
     for _, variant in variants.iterrows():
         row = {
-            'variant': variant['variant'],
-            'nucleotide_index': variant['nucleotide_index'],
-            'gene_name': variant['gene_name'],
-            'gene_position': variant['gene_position'],
-            'codon_idx': variant['codon_idx'],
+            'variant': variant['variant'] if pd.notnull(variant['variant']) else None,
+            'nucleotide_index': variant['nucleotide_index'] if pd.notnull(variant['nucleotide_index']) else None,
+            'gene_name': variant['gene_name'] if pd.notnull(variant['gene_name']) else None,
+            'gene_position': variant['gene_position'] if pd.notnull(variant['gene_position']) else None,
+            'codon_idx': variant['codon_idx'] if pd.notnull(variant['codon_idx']) else None,
             'vcf_evidence': json.loads(variant['vcf_evidence']),
-            'vcf_idx': variant['vcf_idx']
+            'vcf_idx': variant['vcf_idx'] if pd.notnull(variant['vcf_idx']) else None
         }
         _variants.append(row)
     data['variants'] = _variants
 
     #Depending on mutations/effects, populate
     _mutations = []
     if mutations is not None:
         for _, mutation in mutations.iterrows():
             row = {
-                'mutation': mutation['mutation'],
-                'gene': mutation['gene'],
-                'gene_position': mutation['gene_position'],
+                'mutation': mutation['mutation'] if pd.notnull(mutation['mutation']) else None,
+                'gene': mutation['gene'] if pd.notnull(mutation['gene']) else None,
+                'gene_position': mutation['gene_position'] if pd.notnull(mutation['gene_position']) else None,
             }
             if mutation['mutation'][0].isupper() or mutation['mutation'][0] == "!":
                 #Only add codon ref/alt for AA changes
-                row['ref'] = mutation['ref']
-                row['alt'] = mutation['alt']
+                row['ref'] = mutation['ref'] if pd.notnull(mutation['ref']) else None
+                row['alt'] = mutation['alt'] if pd.notnull(mutation['alt']) else None
             _mutations.append(row)
-        data['mutations'] = _mutations
+    data['mutations'] = _mutations
 
     _effects = defaultdict(list)
     antibiogram = {}
     drugs = set()
     if effects is not None and len(effects) > 0:
         for _, effect in effects.iterrows():
             prediction = {
-                'gene': effect['gene'],
-                'mutation': effect['mutation'],
-                'prediction': effect['prediction'],
+                'gene': effect['gene'] if pd.notnull(effect['gene']) else None,
+                'mutation': effect['mutation'] if pd.notnull(effect['mutation']) else None,
+                'prediction': effect['prediction'] if pd.notnull(effect['prediction']) else None,
                 'evidence': {}
             }
             _effects[effect['drug']].append(prediction)
         
         #Get the overall predictions for each drug
         for drug, predictions in _effects.items():
             phenotype = 'S'
@@ -946,18 +1068,18 @@
                 #Use the prediction heierarchy to use most signifiant prediction
                 if values.index(prediction['prediction']) < values.index(phenotype):
                     #The prediction is closer to the start of the values list, so should take priority
                     phenotype = prediction['prediction']
             _effects[drug].append({'phenotype': phenotype})
             antibiogram[drug] = phenotype
             drugs.add(drug)
-        data['effects'] = _effects
+    data['effects'] = _effects
     if catalogue is not None:
         for d in catalogue.catalogue.drugs:
             if d not in drugs:
                 antibiogram[d] = "S"
-        data['antibiogram'] = antibiogram
+    data['antibiogram'] = antibiogram
 
     #Convert fields to a list so it can be json serialised
     with open(os.path.join(path, f'{guid}.gnomonicus-out.json'), 'w') as f:
         f.write(json.dumps({'meta': meta, 'data': data}, indent=2))
```

### Comparing `gnomonicus-2.0.0/gnomonicus.egg-info/PKG-INFO` & `gnomonicus-2.1.0/gnomonicus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomonicus
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 Home-page: https://github.com/oxfordmmm/gnomonicus
 Author: Philip W Fowler, Jeremy Westhead
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford License, see LICENSE
 Keywords: gnomonicus,piezo,lodestone,clockwork,TB
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gnomonicus-2.0.0/setup.cfg` & `gnomonicus-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gnomonicus
-version = 2.0.0
+version = 2.1.0
 author = Philip W Fowler, Jeremy Westhead
 author_email = philip.fowler@ndm.ox.ac.uk
 description = Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/oxfordmmm/gnomonicus
 keywords = gnomonicus, piezo, lodestone, clockwork, TB
@@ -12,16 +12,16 @@
 classifiers = Programming Language :: Python :: 3
 
 [options]
 package_dir = 
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	gumpy>=1.2.1
-	piezo>=0.5
+	gumpy>=1.2.2
+	piezo>=0.6
 	numpy
 	pandas
 	recursive_diff
 zip_safe = False
 include_package_data = True
 scripts = bin/gnomonicus, bin/gbkToPkl
```

