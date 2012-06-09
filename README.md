OntologySimilarity
==================
@LICENSE see LLICENSE file

@authors OntologySimilarity : Alok Dhamanaskar, Michael Cotterell, Rui Wang
@authors OntologyManager : Yung Long Lee
@authors stringMatcher : Akshay Choche

The implementaion of the algorithm is based on Concept SImilarity explained  in Rui Wang's paper  ( Ranking-Based Suggestion Algorithms for Semantic Web Service Composition )

 * The Package OntologySimilarity provides functionality to calculate a similarity score between two concepts in the same Ontology. It considers both syntactic and logical definition of an OWL Class.
 * It takes into account:
	+ Relative Position of two concepts in the Ontology (Coverage Score)
	+ Sentactic Definition (Defintion + Label) (Syntactic Score)
	+ Properties and restrictions on them for the OWL class in consideration
 * The main Package OntologySimilarity has two Internal Dependancies: OntologyManger (For Loading and processing the Ontology), And StringMetrics.
 * Ontology Manager uses OWLAPI (http://owlapi.sourceforge.net/) to load the Ontology, its imports, and retrieve various aspects of an OWL class required for computation of the Similarity

* For testing use :
	ontologySimilarityOntologySimilarityImpl.java Class
	For Printing out the intermediate steps and subscore set
	static final Level debug = Level.INFO;



