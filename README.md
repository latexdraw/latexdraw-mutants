latexdraw Mutants
=================

**Description**


This repository contains mutants of the interactive system LaTeXDraw (http://latexdraw.sourceforge.net/).
These mutants are freely available and can be used for benchmarking GUI testing tools.

Each folder corresponds to one mutant.
The README file in each folder describes:
- The mutant: the code modified to introduce the error; the fault concerned by the mutant
- How to reproduce the failure
- The oracle: how to identify the failure

A patch corresponding to the diff between the reference version of LaTeXDraw and each mutant is also provided at the root folder of each mutant.

**Requirements**

Compiling each mutant requires Java 7 and Maven. To launch the build, go at the root folder of each mutant (where the file pom.xml is located), and launch the command <code>mvn clean package</code>.
The executable file is located in the folder <code>target</code>, in the archive <code>LaTeXDraw-3.0.0-mutantXXX-bin.zip</code>.

**Running the Mutants**

Running the application requires Java 7. Unzip the file <code>LaTeXDraw-3.0.0-mutantXXX-bin.zip</code> and go into the folder <code>data</code> to run the jar file <code>LaTeXDraw.jar</code> (<code>java -jar LaTeXDraw.jar</code>).

**Studying the code**

LaTeXDraw is developed in Java and Scala. The sources of each mutants are located in their folder.
Their code can be imported into the Eclipse IDE (version 4.4 expected + the Scala plug-in).
