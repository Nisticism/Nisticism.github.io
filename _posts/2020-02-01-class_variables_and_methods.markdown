---
layout: post
title:      "Class Variables and Methods"
date:       2020-02-02 01:15:18 +0000
permalink:  class_variables_and_methods
---


Variables and methods are some of the smallest elements of code in almost all languages.  They are the building blocks of any program.  

Within a class, variables and methods can be declared and are called members of the class.  These newly defined objects are sometimes called instance variables and instance methods, as each instance of the class will have its own copies of them.  Unless otherwise specified, if defined within the class, they become instance variable and methods automatically.  Instances of classes may never be used if the class is only called once.  In this case, the functionality of making the class variable or method would serve a precautionary measure in case instances of the class were  created.  This tends to be why class variables and methods are far more commonly used than global variables and methods.  

Variables and Methods in this circumstance are in contrast to global methods and global variables.  These would be universal variables that remain through all classes within the scope of the program.  

Additionally, in some languages, other key words such as static can be applied to variables and methods at the time of creation.  The static key word simply means they cannot be changed, or overwritten at any point during their lifetime.  Of course 

In Java, the key word private indicates before a variable definition, that the variable will be only for that particular class and not for all classes.  The same goes for methods.  If made public, the variable or method would apply to all instance of the class, and be altered whenever a single instance changes its value, as is the case with all non-instance variables or methods.  




