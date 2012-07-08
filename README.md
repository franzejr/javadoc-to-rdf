#Javadoc to RDF

Implementation from MIT Javadoc RDFizer (http://simile.mit.edu/wiki/Javadoc_RDFizer) using Spring Framework as Example.

#How to use

Put your files in a package and change the build.xml in the attribute *dir* puting your java package where the files are in.

<fileset dir="src/org/springframework/beans" defaultexcludes="yes">
              <include name="**"/>
</fileset>

##Using ant

You need ant installed. [Get it from http://ant.apache.org if 
you don't have it installed.]

Second, run "ant" where the build.xml file is located (alongside this very 
document). This will generate a jar file called "rdf_doclet.jar" and then
use it as a doclet to generate an RDF javadoc of the doclet source code in
the './javadoc' folder.

Look into the build.xml file on how to use the doclet on your own ant
build scripts.

##Fork from RDFizer

This is a fork from RDFizer(http://simile.mit.edu/wiki/Javadoc_RDFizer) and is licensed by
Creative Commons Attribution 2.5 Generic(http://creativecommons.org/licenses/by/2.5/)