# definition_identification_classification_naming

Shareable thoughts on these different concepts


When talking about cell classes (cell types or cell states, or cell identities or similar), at least seven concepts are discernible, with different meanings and implications:

1. Clustering: Grouping a sample of observations of cells so as to discern groups of similar observations
2. Describing: Reporting classes of cells that share something in common. A theoretical class that has instances in the real world and predictive values
3. Naming: Choosing a name for this previously reported class of cells. Identifiers are a special kind of computer-readable name. 
4. Classifying: Organizing previously described classes of cells under a common system.
5. Defining: Delimiting rigorously a class of cells, enabling later identification and organizing in logical systems. 
6. Determining: The assignment of cells in experiments to previously defined classes. 
7. Annotating: The recording of metadata associating a cell observation with a unique identifier or name for a class

The  _words_ used above are not, however, used to express only one of those meanings. They are more often than not mixed in the literature. 

Here, I argue there is a benefit in converging on a common and precise vocabulary, to avoid confusion and streamline research. 

In particular, in the context of the Human Cell Atlas, one may find people working with: 

1. Clustering
  Unsupervised clustering is a method for analyzing a dataset. It is about _observations_, but does not say anything directly about the external world, about the rest of reality. 

  Clustering can be used as an intermediary step for _determination_,  i.e.,  assigning names for the  _observations_ (or _events_) in a single-cell / single-nucleus dataset.

  Clustering can be used as initial evidence for the existence of groups of very similar cells. If this group is distinct, it may lead to a _description_.


  This is part of the standard single-cell transcriptomics analysis workflows, and done by data analystics running, e.g. an [scverse pipeline](https://scverse-tutorials.readthedocs.io/en/latest/notebooks/basic-scrna-tutorial.html). 

  
 3. Describing

   Claiming that there are some cells in the world that share a particular kind of similarity, and providing evidence for the existence of this distinguishable class.
   
   Technically, a class is expected to have _instances_, individuals in the real world that can be assigned to this class. 

   In an analogy to taxonomy, clustering is collecting and describing a set of specimens. Describing is concluding from those specimens that there exists a new species.
   
   The description is the jump from detailed observation to theoretical constructs about the world, to identifying groups of things that share so much in common that they deserve a name. 

  _Descriptions_ may be called _discoveries_ if the class has not been recognized before. 

  The description of new classes of cells is part of a publication, though not always as clearly as in the species taxonomy world. The [description of the ionocyte](https://www.nature.com/articles/s41586-018-0393-7) is a good example. 

  Researches describing a class of cell usually go through a _naming_ process to label this class. 
   
 
3. Naming

Naming is the process of selecting words to represent concepts. Here I distinguish two types of naming: human-oriented naming and data-oriented naming. 

Human-oriented naming deals with natural language constructs and may range from informal names to controlled vocabularies. Data-oriented naming provides unique, parseable identifiers for classes, amenable to data processing. 

Species taxonomy represents a special case where the human-oriented names and the data-oriented names were _merged_ in language-based unique identifiers.
The same happens for the Human Genome Nomenclature Consortium (HGNC), which assign short, readable acronyms to genes. 
On the other hand, Ensembl adopts a [data-oriented naming schema](https://www.ensembl.org/info/genome/stable_ids/index.html), maximizing interoperability over communication. 

For other entities, human-oriented naming and data-oriented naming are split. 
For diseases, for example, data-oriented naming includes assigning [ICD Codes](https://en.wikipedia.org/wiki/International_Classification_of_Diseases) for a particular class. But human-oriented naming is looser and will be, at least, language-dependent and more ambiguous. 


3.1 Human-oriented naming 
  Human-oriented naming  schemes are bound to natural languages, and the same classes usually have many different names. 

  For example, the species _Canis familiaris_  is a class of animals corresponding to "dogs" in English, "perros" in Spanish, "cães" in Portugues, "cane" in Italian. 

  Traditional naming, thus, is a process that has a heavy human component: it is a task of finding a word that people will be pleased to call a cell class. 

  There are sometimes even disputes over names: people clash over what, e.g., an "astrocyte" is. That is often a clash over which class of cells deserves the name of "astrocytes". 

  Names are roles for classes. In a diverse world, such as the one of cell biology, adequate naming systems are essential. 
  
  There is not, currently, any standardized  human-oriented naming scheme for cell types. 

3.2 Data-oriented naming

For species, Linneus set up a scientific nomenclature scheme for taxons. Names adhere to certain rules to ensure standardization and uniqueness. Currently, bodies like the International Commission on Zoological Nomenclature and the International Code of Nomenclature for algae, fungi, and plants make sure the naming rules are clear and applied precisely. Names may be considered illegitimate if they don't follow the naming schema. 

Species names act at the same time as _unique identifiers_ for a class and something that is readable for humans. The readability and ethymological meaning of terms facilitate their use by humans. If Linneus called humans SPECIES_9606, perhaps not many people would have adhered to that standard. NCBI, however, does call humans "9606", and that is even more useful for data processing than just _Homo sapiens_.

In the past 300 years, however, the production of knowledge has accelerated. It has gotten to hard to come up with identifiers that are also meaningful and readable. 

The Cell Ontology is, currently, the leading project attempting to provide data-oriented names (or _identifiers_) for cells. They also provide unique labels in English for each of the classes, which work as a more human-friendly proxy . 


After _describing_ and _naming_ a particular cell class, a researcher may be interested in _classifying_ it, e.g., organizing it in a hierarchy of relations. 

4. Classifying

Classifying is the act of organizing cell classes in a hierarchy based on shared traits to improve understanding and data processing. 

This may be done by researchers in reviews and textbooks, doing diagrams and tables. 

In the context of data, the Cell Ontology is, currently, the leading project attempting to provide data-oriented classifications (_hierarchies_) of cells. 

Of note, cell classes don't need to be classified as a single-hierarchy, as there are multiple aspects of similiarity and no reason for them to be naturally in a tree-like structure. 
The Cell Ontology organizes cells a poli-hierarchy, for example. 

5. Defining

  In the context of ontologies, besides human-readable descriptions, classes are assigned precise definitions. 
  In the species taxonomy world, instead of a textual definition, descriptions are backed by real-world specimen vouchers that hold the ground truth.
  The taxonomic descriptions (also called _treatments_) act as rules that base, for example, species identification keys. 
  
  For genes and proteins, this ground truth often comes not from an individual, but a particular reference sequence assigned by a trusted biocuration organization, like UniProt.

  Without a definition, classes lack clearer, discernible ways of finding its instances in the world. A definition, thus, is the process of setting the limits, the boundaries of a class.
  
  The Cell Ontology, for example, strives to transform loose descriptions of cell classes into computable definitions. 
  
 5. Determination

The determination (which may be called also _identification_, _assignment_ or _calling_)  is the process of looking at a cell and stating that it is an _instance of_ some class. The class is referred to by its name, ideally a unique identifiers.

In taxonomy would be looking at an animal, going through a dichotomous key and saying "this individual is a _Canis lupus_". 

In DNA sequencing, looking at particular signals and saying that they correspond to the nucleotide A,T, C or G is called _base calling_, which is an automated kind of determination. 

A range of tools is available to help researchers determine classes of cells, some recently supported by LLMs, for example. Determining the identities of cells is also an important step in single-cell analysis workflows. 

_Determination_ of the classes comes right before _annotation_, the process by which determinations are consolidated into metadata for archiving, processing or sharing. 


6. Annotation 

After one determines which classes are assigned to each observations, one needs to record this relation in an organized manner. 

The process of determination is about making a decision: that cell belongs to class X. 
The process of annotation is telling the world (or your computer) about that decision. 

It might be a color coding scheme + a legend in a figure, it might be a table in a supplementary file that connects observation IDs to class identifiers. 

Improving annotation is improving the _scheme_ of reporting identifications. 

This is a separate activity, because good determination and good annotation are related, but different beasts. 

A dataset with cell labels written in Chinese, and no other language, may be perfectly determined, but perhaps not well annotated. 

Good annotation entails having metadata formats that enable sharing determinations with precise, unique, parseable names, which can be integrated with other bodies of data.

These names, ideally, are linked to a reference classification, such as the identifiers provided by the Cell Ontology. 




  
