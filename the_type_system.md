# The type system
The Luna's type system has the following characteristics:

####Static type system
Luna is a statically typed language, which means that the type of every expression is known at compile time. The type safety leads to safer code and is the foundation for the creation of robust, maintainable systems. It is much better approach than relying on run-time errors, like many languages do nowadays, because a lot of possible errors are caught at compile time. You can be sure that if a program compiles, it does not contain any type based errors, like adding a number and a cake (unless you provide any sensible description how to add 5 to a bun)!

####Dependent types
Luna is a dependent type language. It means, that types and values live in the same space, can be mixed and that types can depend on the values. For example Luna understands how many elements a list stories or what keys are available in a dictionary. In fact Luna understand such relations for every user defined datatype without any explicit code. Luna was designed to understand as much as possible to provide best in class machinery proving that a particular program will work correctly under given conditions. Dependent types are a wide research subject and we are constantly working on extending the possibilities in Luna as much as possible.

####Honesty
Luna's type system is an honest one. This informal term means that the type system does not cheats you! In other words, Luna's type system provides mechanisms for describing the detailed system behavior, including the function purity and possible error occurrence. In Luna you can use type system to indicate that a particular function is pure and does not communicate with any resources external to the program, like all the I/O operations. Such functionality enables Luna to allow many uncommon features, like automatic data parallelism on multicore CPUs and GPUs or support for Software Transactional Memory (STM). There is a great video by Erik Meijer about modern functional language features and the type system honesty: https://www.youtube.com/watch?t=678&v=z0N1aZ6SnBk.




