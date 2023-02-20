
## The Java Virtual Machine

### High-level Programming Languages

- Languages such as Java, C++ and Python.
- Must be translated to machine language before a computer can understand and execute these programs.

### Compiler

- Translates a high-level language into a machine-language program that is executable by your computer.
- Since each computer has its own machine language, the same program must be compiled seperately for each computer it is to run on.
- Complex to create.

### Interpreter

- An alternative to a compiler that is relatively easier to create.
- Translates a program instruction-by-instruction as neccessary, in a similar fashion to a CPU's fetch-and-execute cycle.
- Can be used as emulators to run programs meant for one computer on another.

### Java Virtual Machine (JVM)

- A virtual computer with its own dedicated machine language called Java Bytecode.
- Any computer (MacOS, Windows, Linux, etc) that has a Java Bytecode Interpreter can run the JVM.
- The Bytecode interpreter simulates the JVM, so the program is not technically running on your CPU itself, but via an emulator.
- This allows programmers to only have to compile their code once for any computer, allowing their programs to run on any computer.
- Other languages require their code to be compiled seperately for each type of computer it is to be run on.

#### How the JVM Works:

1. Java program is compiled to Java Bytecode.
2. Bytecode is then interpreted by your computer's specific Bytecode interpreter.
3. As the program is interpreted it is emulated in the JVM.

![JVM Interpretation Diagram](/images/jvm-interpreter-diagram.jpg)

#### Advantages of JVM

- Creating a dedicated Java compiler for each type of computer is complex, whereas creating the Bytecode Interpreter is much more simple.
- Since the program is being run as an emulation, the Bytecode Interpreter acts as a buffer against security threats from downloaded files for all computers on your network.
- Creates ease-of-use for java programmers.

### Just-In-Time Compilers

- One downfall of Java programs were their lack of speed in comparison to other languages that don't run their programs as an emulation.
- Just-in-time compilers act as a solution to this by taking instructions from java programs that will be run multiple times as the program is used, and compiling them into your computer's native machine language so that they are executed much faster.
- Increases overall execution speed.

###### Sources:

Eck, D. J. (2022). *Introduction to Programming Using Java Version 9, JavaFX Edition.* Hobart and William Smith Colleges.

Available [here](https://math.hws.edu/javanotes/?fbclid=IwAR3V0pxqmqNeSpasvbbVrx-RAylNmYW7yYnD2q8-1nJMHErQxynK27MNOhw)

[Next](/topics/introduction-to-java-programming/fundamental-building-blocks.md) [Previous](/readme.md)