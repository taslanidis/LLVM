# LLVM
This project is divided in two parts.<br>
1. Static Checking (Semantic Analysis) for the MiniJava grammar.<br>
2. Convert MiniJava code into the intermediate representation used by the LLVM compiler project.<br>
<br>
<ul>
  <li><b>STMap.java</b> contains all the methods and structures I used for the Symbol Tables.<br>
  <li><b>ScopeVisitor.java</b> and <b>TypeCheckVisitor.java</b> is the first two passes on the parse tree who perform the <b>Semantic Analysis</b>.<br>
  <li><b>LlvmVisitor.java</b> does one pass on the tree and generates the intermediate code.<br>
</ul>
<br>
About the visitors, as stated in the project: <br>
<i>"The visitors you will build should be subclasses of the visitors generated by JTB, but they may also contain methods and fields to hold information during static checking, to transfer information from one visitor to the next, etc. In the end, you will have a Main class that runs the semantic analysis initiating the parser that was produced by JavaCC and executing the visitors you wrote. You will turn in your grammar file, if you have made changes, otherwise just the code produced by JavaCC and JTB alongside your own classes that implement the visitors, etc. and a Main. The Main should parse and statically check all the MiniJava files that are given as arguments."</i>
<br><br>
Project for the course "Compilers K31".
