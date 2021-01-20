# CoCEC
Source code of tool Combinational Circuit Equivalence Checker (CoCEC). CoCEC checks functional equivalence of two combinational circuits automatically. 

Installation

 To run and experiment with CoCEC tool, follow these steps:

  1) download and save the source of CoCEC (folder 'CoCEC-v0')
  2) install Coq (version 8.8) and add its path to environment variables
  3) install g++ compiler and add its path to environment variables
  4) enter the folder containing the source of the tool CoCEC (cd CoCEC-v0)
  
  In Windows:
  5-a) run the g++ compiler on the main-win.cpp as the following:
     C:\CoCEC-v0>g++ main-win.cpp -o main-win -enable-auto-import -lcomdlg32 basicfuns.cpp syntaxchecker.cpp
        proofchecker.cpp irgenerator.cpp codegenerator.cpp parser.cpp

	The option '-lcomdlg32' is added for 'GetOpenFileName(&ofn)'
  In Ubunto:
  5-b) run the g++ compiler on the main-ubunto.cpp as the following:
     C:\CoCEC-v0>g++ main-ubunto.cpp -o main-ubunto -enable-auto-import -lcomdlg32 basicfuns.cpp syntaxchecker.cpp
        proofchecker.cpp irgenerator.cpp codegenerator.cpp parser.cpp
  6) run the main-win.exe/main-ubunto.exe file.

  Two combinational circuits can be typed in the two input boxes and their equivalence is checked by clicking the button 'Check Equivalence'. 
  Alternatively, circuit descriptions can also be loaded using the two load buttons. 
  CoCEC stores the Coq proof script in 'proofscript.v' file, Coq proof object/term in 'proofobject.txt',
  counter-example in 'counterexample.txt' and Coq error in 'coqerror.txt' files. The Window
  version additionally records verification time in 'statistics.txt'.  
