1.1 Basic Programming Model
---
### Basic structure of a Java program
### Primitive data types and expressions
* *Precedence* convention
	* logical operators: `!` > `&&` > `||`


### Statements
### Shortcut notations
### Arrays
* Aliasing
		
		int[] a = new int[N];
		...
		int[] b = a;


### Static methods
* Arguments are passed by value.
* Recursion. Three important rules of thumb:
	* The recursion has a base case.
	* Recursive calls must address subproblems that are smaller.
	* Recursive calls should not address subproblems that overlap.
* Unit testing.
	> A best practice in Java programming is to include a `main()` in every library of static methods that tests the methods in the library.

### APIs
* Your own libraries.
	> It is worthwhile to consider *every program that you write* as a library implementation, for possible reuse in the future.


### Strings
* `String` is *not* a primitive type.
* Automatic Conversion
	* if *one* of the arguments of + is a String, Java *automatically* converts the other argument to a String. (`toString() method`)

### Input and output
* Formatted output.
	* `printf(format string, content)`
	* format string: begins with %, ends with a one-letter *converstion code* (d: decimal values of int, f, s: String)
	* between the % and the conversion code is an integer value that specifies the *field width* of the converted value (number of characters).
	* By default, blank space added on the left; insert minus sign to make it right.
	* period followed by the number of digits to put after the decimal point for a `double` value or the number of beginning characters of `String`.
	
* Redirection and piping.

### Binary Search Example

Exercises
---
**1.1.3** Compare two strings: `String1.equals(String2)`

**1.1.9** Put the binary representations of a positive integer N into a `String` `s` (including 2 subproblem).

* **Think from the other side.**
	``` java
	String s = "";
	for (int n = N; n > 0; n /= 2)
		s = (n % 2) + s;
	```



