
## The Basic Java Application

### Programming Languages

- Must be unambiguous.
- Has strict rules on what is, and what is not, allowed.

### Syntax

- Determines what is allowed.
- Specifies vocabulary and how programs are constructed (branches, loops, etc).
- "Syntactically correct" means the program is constructed properly and is able to be compiled.

### Semantics

- The "meaning" of a program - does it produce the intended result when executed?
- "Semantically correct" means the program does what you intended it to do.

### Pragmatics

- The "style" put into your program.
- The program is written in a way that is easy to read and understand by others.
- Computers don't care about pragmatics and can technically run a program written entirely on one line.
- The formatting, comments, etc of your program are important for not only you to be able to understand what is being written, but others that may be assissting in the project as well.

### Basic Programming Process

1. Get the program text into the computer.
2. Compile the program.
3. Run the compiled program.

### "Hello World" Java Program

![Java Program Example](/images/hello-world.jpg)

#### Subroutine Call Statements

- A statement that uses the name of a subroutine to "activate" it to accomplish a task.
- In the above example, "System.out.println" is the subroutine being called on to display the message "Hello World!". 

#### Built-in Subroutine

- A subroutine that is a pre-defined part of the programming language itself, allowing it to be called on without any extra steps.
- In this case, "System.out.println" would be a built-in subroutine.

#### public class HelloWorld {}

- This line establishes the class "Hello World", and doubles as the program name as well.
- All Java programming is done within classes, and as such, a subroutine cannot exist outside one.
- Not all classes are programs.

#### public static void main(String[] args) {}

- This line establishes the class as a program using the subroutine "main()".

#### "main()" Subroutine

- This is the subroutine that tells the java interpreter that this class is a program, and allows it to execute the enclosed instructions.

#### "public"

- "public" on the line of main() allows the main() subroutine to be called on from outside the program. 
- This is necessary since the Java interpreter, which is translating the program to be executed, is external to the program itself.

#### Comments

- Comments are notes written into the program for other humans to read, that the computer ignores.
- This is an essential part of pragmatics.
- There are three types of comments:
1. // signifies a comment that spans only a single line.
2. Comments that span multiple lines will begin with /* and end with */, with a single * on each line inbetween.
3. Comments beginning with /** are Javadoc comments used for producing documentation.

### Saving and Compiling

- If the class name is HelloWorld, then it must be saved as HelloWorld.java. 
- Once compiled, the translated program will appear as a file called HelloWorld.class.
- .java files are the source code, and .class files are the files needed to actually run the program.

### Packages

- Packages are groups of classes.

###### Sources

Eck, D. J. (2022). *Introduction to Programming Using Java Version 9, JavaFX Edition.* Hobart and William Smith Colleges.

Available [here](https://math.hws.edu/javanotes/?fbclid=IwAR3V0pxqmqNeSpasvbbVrx-RAylNmYW7yYnD2q8-1nJMHErQxynK27MNOhw)

[Previous Section](/topics/introduction-to-java-programming/the-mental-landscape/internet-and-beyond.md) | [Home](/readme.md)


<table>
	<caption>Primitive Types</caption>
	<thead>
		<tr>
			<th>Name</th>
			<th>Data Type</th>
		</tr>
	</thead>

	<tbody>
		<tr>
			<td>byte</td>
			<td rowspan = "4">Integer Type</td>
		</tr>
		<tr>
			<td>short</td>
		</tr>
		<tr>
			<td>int</td>
		</tr>
		<tr>
			<td>long</td>
		</tr>
		<tr>
			<td>float</td>
			<td rowspan = "2">Real Number</td>
		</tr>
		<tr>
			<td>double</td>
		</tr>
		<tr>
			<td>char</td>
			<td>Single Character</td>
		</tr>
		<tr>
			<td>boolean</td>
			<td>Logical Values: True or False</td>
		</tr>
	</tbody>
</table>

