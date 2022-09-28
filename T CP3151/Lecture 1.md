# Introduction to Integrative Programming

### Difference between Compiler and Interpreter
1. A **Compiler** will scan and translate source codes in whole (such as C/C++, JAVA, Objective-C language) into machine language (binary number such as `0` and `1`) which will generate an `.exe` file at the end of compiling.
2. **Compiler** takes time to analyse the source codes (such as C/C++, JAVA, Objective-C language). It generates all the errors at the end of compilation, making debugging difficult. However, the time taken to execute the process is much quicker than Interpreter.
	 A given example will be, the compiler generates errors messages for `Section A`, `Section B`, and `Section C`. As a matter of fact, it is just the error in the `A Section`, causing B and C to generate errors. Thus, making the debugging process difficult. 
3. An **Interpreter** translates program code (such as Python, JavaScript, PHP) into machine code. It translates just one statement of the program at a time (equivalent to line by line).