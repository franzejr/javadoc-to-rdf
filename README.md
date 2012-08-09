#Javadoc to RDF

Implementation from MIT Javadoc RDFizer (http://simile.mit.edu/wiki/Javadoc_RDFizer) using Spring Framework as Example.

#How to use

You need to use this script:

javadoc -sourcepath src -doclet edu.mit.simile.rdfizer.javadoc.RDFizerDoclet -out <yourRDFName>.rdf -docletpath rdf_doclet.jar <your.package.br>
	
Example:

javadoc -sourcepath src -doclet edu.mit.simile.rdfizer.javadoc.RDFizerDoclet -out javadoc.rdf -docletpath rdf_doclet.jar org.springframework.beans

So, you must to put the rdf_doclet.jar in your directory and set the package's name you want to use.

Or you may use the run.sh script passing by parameter the packagename

Example:

./run.sh org.springframework.beans

##Fork from RDFizer

This is a fork from RDFizer(http://simile.mit.edu/wiki/Javadoc_RDFizer) and is licensed by
Creative Commons Attribution 2.5 Generic(http://creativecommons.org/licenses/by/2.5/)