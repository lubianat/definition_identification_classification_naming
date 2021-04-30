# definition_identification_classification_naming

Shareable thoughts on these different concepts


When talking about cell types, at least four concepts are discernible, with different meanings and implications:

1. Clustering: Grouping a sample of observations of cells so as to discern groups of similar observations
2. Classification: Reporting classes of cells that share something in common. Crafting a new type, a new theoretical class that has instances in the real world and predictive values
3. Naming: Choosing a name for this previously reported class of cells
4. Definition: Delimiting a classification of cells so as to be able to identify them later
5. Identification: The assignment of cells in experiments to previously defined classes. 
6. Annotation: The recording of metadata associating a cell observation to the identifier for a class


The four _words_ used above are not, however, used to express only one of those meanings. 

They are more often than not mixed in the literature. 


Here, I argue there is a benefit on converging on a common and precise vocabulary, to avoid confusion and streamline research. 

In special in the context of the human cell atlas. 

1. Clustering
  Performing unsupervised clustering is a way to analyze a dataset. It is about _observations_, but does not say anything about the external world, about the rest of reality. 
  Clustering can be a basis for classification (2).
  Clustering can be used as an heuristic to assign _observations_ in a dataset to classes of cells. 
  
 2. Classification / conceptualization
   Claiming that there are cells generally, in the world, that share some kind of similarity. That are a part of a common class. 
   Looking at clusters, a researcher may hypothesize that in other samples, other cells may share the same characteristics. 
   Technically, a class is expected to have _instances_, individuals in the real world that can be assign to this class. 
   In an analogy to taxonomy, clustering is collecting and describing a set samples. Classification is concluding  from those samples that there is a new species.
   The classification is the jump from observation to general theories, to conceptualizations about the world.
   
 
3. Naming

Naming is the process of selecting words to represent concepts. Here I distinguish two types of naming: traditional naming and formal naming. 

3.1 Traditional naming 
  Traditional naming schemes are bound to natural languages, and the same classes usually have many different names. 

  For example, the species _Canis familiaris_  is a class of animals corresponding to "dogs" in English, "perros" in Spanish, "cães" in Portugues, "cane" in Italian. 

  Traditional naming, thus, is a process that has a heavy human component: it is a task of finding a word that people will be pleased to call a cell class. 

  There is, sometimes, even disputes over names: people clash over what, e.g., an "astrocyte" is. That is often a clash over which class of cells deserves the name of "astrocytes". 

  Names are rotules for classes. In a diverse world, such as the one of cell biology, adequate naming systems are very important. 
  There is not, currently, any standardizing naming scheme for cell types. 

3.2 Formal naming

For species, Linneus set up a scientific nomenclature scheme for taxons. Names adhere to certain rules to ensure standardization and uniqueness. Currently, bodies like the International Commission on Zoological Nomenclature refine the standards. 

Species names acts at the same time as _unique identifiers_ for a class and something that is readable for humans. The readability and ethymological meaning of terms facilitate their use by humans. If Linneus called humans SPECIES_08375, perhaps not many people would have adhere to that standard. 

In the past 300 years, however, the production of knowledge has accelerated. It has gotten to hard to come up with identifiers that are also meaningful and readable. 

Thus, generally hereas for species we have species names in Latin that are unique (no two species should have the same name), for other concepts, ontologists assign identifiers. 

The assignment of identifiers in OBO Foundry ontologies is independent of the definition of the class. It is a fashion of "formal naming" that greatly  facilitates classification. 

Classes can receive either formal names, traditional names or no names at all (what is called technically an "anonymous class")

4. Definition
  It is possible to craft a class without an specific definition.
  An undefined class does not have clear, discernible ways of finding its instances in the world. 
  A definition, thus, is the process of setting the limits, the boundaries of a class.
  
  This meaning is very close to the one of classification. 
  In that sense, when one defines a "cell type" or a "cell state", one is setting the rules for finding other instances of a class. 
  
  For example, one might claim that cytotoxic lymphocytes are defined by the expression of the CD8A gene. That is a definition. 
  
  One can, however, find a class but not set clear definition limits, for example, by setting a set of "type specimens" in a reference dataset an claiming that "there exists a class similar to this one". 
  
  In any case, I argue that researchers often set classes with loose boundaries, and in other cases (especially in ontology projects) focus on definition, i.e. refining the boundaries common concepts. 
  
 5. Identification 

The identification is the process of looking at a cell an saying that it is an _instance of_ some class. The class is referred to by its name, ideally an unique identifiers.

In taxonomy would be looking at an animal and saying "this is a dog", "this is a class", and so on. 

6. Annotation 

After cell observations are assigned to certain classes, it is important to record this relation in an organized manner. 

The process of identification is about making a decision: that cell belongs to class X. 
The process of annotation is telling the world about that decision. 

It might be a color coding scheme + a legend in a figure, it might be a table in a supplementary file that connects observation IDs to class identifiers. 
Improving annotation is improving the _scheme_ of reporting identifications. 





  
