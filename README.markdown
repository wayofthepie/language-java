language-java 
=============

Haskell parser and pretty printer for the java language.


How to use
----------

Simple compilation unit parser:

    parser compilationUnit "import java.util.*; public class MyClass {}"

or from a file:

    ast <- parser compilationUnit `fmap` readFile "myClass.java"
