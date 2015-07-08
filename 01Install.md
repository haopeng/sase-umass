#This page explains how to install SASE 1.0 on your machine.

Since we developed SASE using Java, a Java Runtime Environment must be installed. The engine also uses libraries which are included in the [SASE package](http://code.google.com/p/sase-umass/downloads/list). We have tested the SASE system on Unix, Mac and Windows(Cygwin).

# Structure of the SASE 1.0 Package #
The structure of the SASE 1.0 package is as follows.



| **COPYRIGHT**  | lists the license under which this package is released.|
|:---------------|:-------------------------------------------------------|
| **INSTALL**        | is a quick installation guide.                         |
| **bin/**       | contains the complied classes.                         |
| **build/**     | contains the JAR file.                                 |
| **doc/**       | contains the Java doc.                                 |
| **examples/**  | contains some quick examples for you to start          |
| **lib/**       | contains the required libraries.                       |
| **src/**       | contains the Java source files                         |
| **tests/**     | contains the queries and data files for a set of experiments |

# Software Requirement #

  * Install the [Java Runtime Environment](http://www.oracle.com/technetwork/java/javase/downloads/index.html) version 1.5.x or later

# Configuration #
(If you are using **Windows**, please install **Cygwin** first.)

Please follow the configuration steps below:

  * Unzip the package you [downloaded](http://code.google.com/p/sase-umass/downloads/list)
  * Set the **SASE\_HOME** environment variable to point to the folder where the unzipped files are placed.
  * Add **$SASE\_HOME/build/sase.jar** to the CLASSPATH
  * Add **$SASE\_HOME/lib/jeval.jar** to the CLASSPATH.
  * Add **$SASE\_HOME/bin** to the PATH to access all the executables.


Next you can run **SASE** by these [commands](http://code.google.com/p/sase-umass/wiki/02RunExperiments).

If you want to modify the source code, the **Main Class** is **edu.umass.cs.sase.UI.CommandLineUI.java**.