OntologySimilarity
==================
@LICENSE see LICENSE file

@authors OntologySimilarity : Alok Dhamanaskar, Michael Cotterell, Rui Wang
@authors OntologyManager : Yung Long Lee
@authors stringMatcher : Akshay Choche

The implementation of the algorithm is based on Concept Similarity explained  in Rui Wang's paper  ( Ranking-Based Suggestion Algorithms for Semantic Web Service Composition )

 * The Package OntologySimilarity provides functionality to calculate a similarity score between two concepts in the same Ontology. It considers both syntactic and logical definition of an OWL Class.
 * It takes into account:
    + Relative Position of two concepts in the Ontology (Coverage Score)
    + Syntactic Definition (Definition + Label) (Syntactic Score)
    + Properties and restrictions on them for the OWL class in consideration
 * The main Package OntologySimilarity has two Internal dependencies: OntologyManger (For Loading and processing the Ontology), And StringMetrics.
 * Ontology Manager uses OWLAPI (http://owlapi.sourceforge.net/) to load the Ontology, its imports, and retrieve various aspects of an OWL class required for computation of the Similarity

 * For testing use :
    ontologySimilarityOntologySimilarityImpl.java Class
    For Printing out the intermediate steps and subscore set
    static final Level debug = Level.INFO;
 * The package has been Tested on ontologies OBI and OBI-WS (http://code.google.com/p/obi-webservice/) and should work well with most ontolofies under BFO.
 * For Other Ontologies, Change relevant annotation properties in ontologyManager.ontologySimilarity.properties Properties file
 


