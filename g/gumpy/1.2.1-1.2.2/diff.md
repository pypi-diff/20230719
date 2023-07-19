# Comparing `tmp/gumpy-1.2.1.tar.gz` & `tmp/gumpy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gumpy-1.2.1.tar", last modified: Fri Jun 30 09:23:53 2023, max compression
+gzip compressed data, was "gumpy-1.2.2.tar", last modified: Wed Jul 19 11:19:35 2023, max compression
```

## Comparing `gumpy-1.2.1.tar` & `gumpy-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-30 09:23:10.000000 gumpy-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 09:23:53.974406 gumpy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-30 09:23:10.000000 gumpy-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 09:23:10.000000 gumpy-1.2.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-06-30 09:23:10.000000 gumpy-1.2.1/bin/gumpy-save-genome.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-06-30 09:23:10.000000 gumpy-1.2.1/bin/to_piezo_catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/gumpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/difference.py
--rw-r--r--   0 runner    (1001) docker     (123)    34070 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/gene.py
--rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/genome.py
--rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-06-30 09:23:10.000000 gumpy-1.2.1/gumpy/variantfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:23:53.974406 gumpy-1.2.1/gumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:23:17.000000 gumpy-1.2.1/gumpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 09:23:53.000000 gumpy-1.2.1/gumpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 09:23:10.000000 gumpy-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-30 09:23:53.974406 gumpy-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:19:35.407678 gumpy-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-19 11:19:00.000000 gumpy-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-19 11:19:35.407678 gumpy-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-19 11:19:00.000000 gumpy-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 11:19:00.000000 gumpy-1.2.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:19:35.407678 gumpy-1.2.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-07-19 11:19:00.000000 gumpy-1.2.2/bin/gumpy-save-genome.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-07-19 11:19:00.000000 gumpy-1.2.2/bin/to_piezo_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:19:35.407678 gumpy-1.2.2/gumpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-19 11:19:00.000000 gumpy-1.2.2/gumpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-07-19 11:19:00.000000 gumpy-1.2.2/gumpy/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36112 2023-07-19 11:19:00.000000 gumpy-1.2.2/gumpy/gene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41105 2023-07-19 11:19:00.000000 gumpy-1.2.2/gumpy/genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29989 2023-07-19 11:19:00.000000 gumpy-1.2.2/gumpy/variantfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:19:35.407678 gumpy-1.2.2/gumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-19 11:19:35.000000 gumpy-1.2.2/gumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-19 11:19:35.000000 gumpy-1.2.2/gumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:19:35.000000 gumpy-1.2.2/gumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:19:06.000000 gumpy-1.2.2/gumpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 11:19:35.000000 gumpy-1.2.2/gumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 11:19:35.000000 gumpy-1.2.2/gumpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-19 11:19:00.000000 gumpy-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-19 11:19:35.407678 gumpy-1.2.2/setup.cfg
```

### Comparing `gumpy-1.2.1/LICENSE` & `gumpy-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.1/PKG-INFO` & `gumpy-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Genetics with Numpy
 Home-page: https://github.com/oxfordmmm/gumpy
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gumpy-1.2.1/README.md` & `gumpy-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.1/bin/gumpy-save-genome.py` & `gumpy-1.2.2/bin/gumpy-save-genome.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.1/bin/to_piezo_catalogue.py` & `gumpy-1.2.2/bin/to_piezo_catalogue.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.1/gumpy/__init__.py` & `gumpy-1.2.2/gumpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.1/gumpy/difference.py` & `gumpy-1.2.2/gumpy/difference.py`

 * *Files identical despite different names*

### Comparing `gumpy-1.2.1/gumpy/gene.py` & `gumpy-1.2.2/gumpy/gene.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,31 +242,62 @@
                         alt = bases[1]
                         mutations.append(ref + str(pos) + alt + ":" + str(populations[0][coverage]))
                 else:
                     self.minor_nc_changes[pos] = nc_changes
                     mutations.append(str(pos) + "_" + type_ + "_" + bases + ":" + str(populations[0][coverage]))
             else:
                 self.minor_nc_changes[gene_pos] = nc_changes
-                #We have a mixture here so report as Zs
-                #Other than if we have conflicting indels at a gene index (in that case, crash)
-                c = Counter([(nc_idx, type_) for nc_idx, type_, bases, cov, frs in gene_pos_map[gene_pos]])
-                for (i, t), count in c.items():
-                    if t in ["ins", "del"] and count > 1:
-                        #We have a single index with > 1 indel so complain
-                        assert False, f"A minor population exists in gene {self.name} which has > 1 indel at gene index {i}!"
+                #We have a mixture here so report as Zs for SNPs, indel for indels, and mixed for mixed indels and SNPs
+                c = Counter([(nc_idx, 'indel') if type_ in ['ins', 'del'] else (nc_idx, type_) for nc_idx, type_, bases, cov, frs in gene_pos_map[gene_pos]])
                 
-                cov = max([pop[coverage] for pop in populations])
-                if self.codes_protein and gene_pos > 0:
-                    #These need a little extra effort to pull out the ref AA
-                    ref = self.codon_to_amino_acid[reference.codons[self.amino_acid_number == gene_pos][0]]
-                    mutations.append(ref + str(gene_pos) + "Z:" + str(cov))
+                #Get the number of indels within this codon/base
+                indels = sum([count for (i, t), count in c.items() if t == "indel"])
+                snps = sum([count for (i, t), count in c.items() if t == "snp"])
+
+                if indels > 0 and snps > 0:
+                    #Mixed within the codon/base so return <pos>_mixed
+                    cov = max([pop[coverage] for pop in populations])
+                    mutations.append(str(gene_pos)+"_mixed:"+str(cov))
+                elif indels > 0:
+                    #Just indels, so return of form <pos>_indel
+                    #Little bit more difficult here as we have to check each nucleotide_number
+                    #   this way, if there is only 1 indel per nucleotide, we can be specific
+                    for (i, t), count in c.items():
+                        if count == 1:
+                            #Exactly 1 indel at this position so be specific
+                            #Use the nc_idx instead of gene_pos as they may not be equal
+                            minor = [
+                                (nc_idx, type_, bases, cov, frs) 
+                                for nc_idx, type_, bases, cov, frs 
+                                in gene_pos_map[gene_pos] 
+                                if nc_idx == i
+                            ][0]
+                            self.minor_nc_changes[minor[0]] = 0
+                            mutations.append(str(minor[0]) + "_" + minor[1] + "_" + minor[2] +":" + str(minor[coverage]))
+                        else:
+                            #>1 indel here, so `<pos>_indel` as as accurate as we can be
+                            minors = [
+                                (nc_idx, type_, bases, cov, frs) 
+                                for nc_idx, type_, bases, cov, frs 
+                                in gene_pos_map[gene_pos] 
+                                if nc_idx == i
+                            ]
+                            self.minor_nc_changes[minors[0][0]] = 0
+                            cov = max([pop[coverage] for pop in minors])
+                            mutations.append(str(minors[0][0])+"_indel:"+str(cov))
                 else:
-                    ref = reference.nucleotide_sequence[self.gene_position == gene_pos][0]
-                    mutations.append(ref + str(gene_pos) + "z:" + str(cov))
-                    
+                    #Just SNPs, so return of form <ref><pos>(z|Z) as appropriate
+                    cov = max([pop[coverage] for pop in populations])
+                    if self.codes_protein and gene_pos > 0:
+                        #These need a little extra effort to pull out the ref AA
+                        ref = self.codon_to_amino_acid[reference.codons[self.amino_acid_number == gene_pos][0]]
+                        mutations.append(ref + str(gene_pos) + "Z:" + str(cov))
+                    else:
+                        ref = reference.nucleotide_sequence[self.gene_position == gene_pos][0]
+                        mutations.append(ref + str(gene_pos) + "z:" + str(cov))
         return sorted(mutations)
 
 
         
     def __revcomp_indel(self) -> None:
         '''Make some adjustments for deletions within revcomp genes. 
         The largest of which is that the gene position of the deletion needs adjusting for revcomp. 
@@ -601,31 +632,31 @@
             valid = valid and int(pos) in self.amino_acid_number
             return valid
 
         #Match indel
         indel = re.compile(r"""
                     ([a-zA-Z_0-9.()]+@)? #Possibly leading gene name
                     (-?[0-9]+) #Position
-                    _(ins|del|indel)_? #Type
+                    _(ins|del|indel|mixed)_? #Type
                     ([0-9]+|[acgtzx]+)? #Bases deleted/inserted
                     """, re.VERBOSE)
         if indel.fullmatch(variant):
             #Variant is an indel
             #Check it is valid
             name, pos, type_, bases = indel.fullmatch(variant).groups()
             valid = True
             pos = int(pos)
             end = numpy.max(self.nucleotide_number)
             #Check the names match
             if name is not None and name != "":
                 valid = valid and name[:-1] == self.name
             #Check pos in correct range
             valid = valid and int(pos) in self.nucleotide_number
-            if type_ == "indel":
-                #If a mutation is given as `indel`, no length/bases should be given
+            if type_ == "indel" or type_ == "mixed":
+                #If a mutation is given as `indel` or `mixed`, no length/bases should be given
                 valid = valid and (bases is None or bases == "")
             if type_ == "del" and bases is not None and bases != "":
                 #Mutation was del, so check if the bases given match the ref
                 if bases.isnumeric():
                     #A length was given rather than bases so just check that all bases are in the correct range
                     if pos < 0:
                         #Is a promoter so be careful about pos+bases not being 0
```

### Comparing `gumpy-1.2.1/gumpy/genome.py` & `gumpy-1.2.2/gumpy/genome.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,16 +844,28 @@
                 else:
                     genome.indel_length[idx-1] = -1*len(vcf.calls[(idx,type_)]['call'][1])
             
             elif type_ == 'ref':
                 #These only exist due to reference calls
                 #They only made it this far as they are required to pull out minors at these positions
                 pass
+        
+        genome.minor_populations = []
 
-        genome.minor_populations = vcf.minor_populations
+        for minor in vcf.minor_populations:
+            #Ensure that the VCF evidence for these is also recorded correctly
+            pos = minor[0]
+            evidence =  minor[5]
+            
+            #Store the VCF evidence of this
+            genome.vcf_evidence[genome.nucleotide_index[pos - 1]] = evidence
+
+            #Don't keep the VCF evidence with this, as it is already stored in the main vcf_evidence dict
+            genome.minor_populations.append(minor[:5])
+            
         genome.vcf_file = vcf
 
         #Let's assign some deleted regions (if exist)
         self.__assign_deleted(genome)
 
         # the genome has been altered so not a reference genome
         genome.is_reference = False
```

### Comparing `gumpy-1.2.1/gumpy/variantfile.py` & `gumpy-1.2.2/gumpy/variantfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,18 @@
         assert 'GT' in record.samples[sample].keys(), 'require GT in FORMAT column to parse genotype'
 
         #Save some of the easier to get to attributes
         self.chrom = record.chrom
         self.contig = record.contig
         self.pos = record.pos
         self.ref = record.ref.lower()
-        self.alts = tuple([i.lower() for i in record.alts])
+        if record.alts is not None:
+            self.alts = tuple([i.lower() for i in record.alts])
+        else:
+            self.alts = None
         self.qual = record.qual
 
         #Get the filter attribute value
         assert len(record.filter.items()) >= 0, "A record has more than 1 filter set!"
         if len(record.filter.items()) == 0:
             self.filter = None
             self.is_filter_pass=False
@@ -314,17 +317,19 @@
 
             #Break down the calls as appropriate
             simple = [self._simplify_call(ref, alt) for alt in calls]
 
             #Map each call to the corresponding read depth
             dps = list(self.calls[(idx, type_)]['original_vcf_row']["COV"])
 
-            total_depth = self.calls[(idx, type_)]['original_vcf_row']['DP']
+            # total_depth = self.calls[(idx, type_)]['original_vcf_row']['DP']
+            total_depth = sum(dps)
             
             #idx here refers to the position of this call, NOT this vcf row, so adjust to avoid shifting when building minor calls
+            original_idx = idx
             idx = idx - self.calls[(idx, type_)]['pos']
             for (calls, depth) in zip(simple, dps):
                 #As we can have >1 call per simple, iter
                 for call in calls:
                     #Check that this call isn't one of the actual calls
                     if (idx+int(call[0]), *call) in simple_calls:
                         #Is an actual call so we skip
@@ -337,15 +342,24 @@
                             #We don't actually care though
                             #This has to be done here as simplifying calls can move the position
                             continue
                         if call[1] == 'snp' and call[2][0] == call[2][1]:
                             #Ref calls aren't interesting
                             continue
                         #Only tracking absolute number of reads
-                        self.minor_populations.append((pos, call[1], call[2], int(depth), round(depth/total_depth, 3)))
+                        self.minor_populations.append(
+                            (
+                                pos, 
+                                call[1], 
+                                call[2], 
+                                int(depth), 
+                                round(depth/total_depth, 3), 
+                                self.calls[(original_idx, type_)]['original_vcf_row']
+                            )
+                        )
         
     def __find_calls(self):
         '''
         Private method to find changes within the genome based on the variant file.
 
         Creates calls dict used elsewhere.
         '''
```

### Comparing `gumpy-1.2.1/gumpy.egg-info/PKG-INFO` & `gumpy-1.2.2/gumpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Genetics with Numpy
 Home-page: https://github.com/oxfordmmm/gumpy
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gumpy-1.2.1/setup.cfg` & `gumpy-1.2.2/setup.cfg`

 * *Files identical despite different names*

