## RC1920-LAB0-CSNN
RC1920-LAB0 CSNN (Computer Networks Simple Simulator)


CNSS (Computer Networks Simple Simulator)
RC2020 Labs will use CNSS for part of the semester. CNSS makes it possible to code and simulate simple networking protocols. The simulation results are deterministic and repeatable, making it easier to reproduce and interpret them.

CNSS is written in Java 8. The source code is publicly available and hosted at GitHub

## How can you obtain the CSNN Simulator ?
Fetching CNSS
For those still unfamiliar with GitHub repositories, there are several ways to access the source code.

You can download a zip archive of the entire repository from here
(https://github.com/jlegatheaux/cnss)

You can also use git (https://git-scm.com/)
to clone the contents of the repository to a local directory, like so:


Double-click (or enter) to edit

$ git clone https://github.com/smduarte/cnss.git

This will create a directory cnss in the current directory with a local repository with the latest version.

You can refresh and update the local repository, by executing the following command in the repository folder:

$ git -C cnss pull

You must see .... 
Already up to date.

## For Eclipse Users
CNSS can also be imported directly to Eclipse.

For version 2020-06, the procedure is as follows:

Copy the CNSS repository uri (https://github.com/jlegatheaux/cnss.git) into the clipboard;
Navigate: File > Import > Git, choose Projects from Git, then Next
Choose Clone URI, then Next twice.
If asked, only select the master branch and press Next until finished.

## Compiling CNSS manually (Console)
CNSS has no external dependencies.

At the root of the repository, the source code can be compiled in the command line (shell), like so:

$ javac -d cnss-classes cnss/CNSS/src/*/*/*.java

Pay attention: i this example you must have csnn directory 
The switch -d cnss-classes will place the resulting classes in the cnss-classesdirectory.

## To run CNSS

You must create a configuration file (in this case it will be empty ... Later you will learn how to use
this file to describe a "network topology".

$ echo > empty.config.txt

And then you are ready to run the simulator using the configuration file as ye given argument

$ java -cp .:cnss-classes cnss.simulator.Simulator empty.config.txt

You will see as ouyput ...

Loading configuration : empty.config.txt
Reading file empty.config.txt

simulation starts - first processing step with clock = 0

simulation ended - last processing step with clock = 0

#End of this part o Lab 0
Great. You concluded your CNSS Simulator installation, you compiled it and it is ready for the next steps.
So .. Go to LAB 0 - Part 2.
