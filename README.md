# 9-31Notes
Java SE Fundamentals Notes Chapters 7-10

Chapter 7 Working with Strings

String - Sequence of Unicode characters
String variables 
- Do not directly store string instance
- Hold a reference to string instance
Strings are immutable 
- Changes in the value create a new string instance
Sting equality 
- prefer the equals method
String interning 
- provides a canonicalized value
- Enables reliable use of == operator
- Improves performance of frequently compared Strings
StringBuilder 
- Provides mutable string buffer
- Efficiently constructs string values
- Use toString to extract string content

Chapter 8 Understanding Classes and Objects

Class 
- Template for creating objects
Object 
- Instance of a class
Classes are reference types 
- Class variables simply hold a reference
- Instances created with new keyword
- Multiple variables can reference the same instance
Fields
- Store object state
Methods
- Executable code
- Manipulate state
- Perform operations
Constructors
- Executable code
- Runs during object creation
- Sets initial state

Special References
this
- Implicit reference to current object
null
- Represents an uncreated object

Access Modifiers
- Control class visibility
- Control member visibility
- Enable encapsulation

Fields not normally directly accessible
- Use methods to provide access
- Accessors retrieve field values
- Mutators modify field values

Chapter 9 Implementing Class Constructors and Initializers

Object initial state
- Initial state expected to be useful
- Java provides default field values

Field initializers
- Set initial value as part of declaration
- Can include an equation, other fields, and method calls

Constructors
- code that runs during object creation
- Accept zero or more parameters
- Can have multiple

One constructor can call another
- Call must be first line of constructor
- Can pass parameters

Constructors can be non-public
- Limits which code can perform specific types of instance creation

Initialization blocks
- code that runs during object creation
- not tied to any specific constructor
- Cannot receive parameters

Chapter 10 Using Static Members

Static Fields
- Values not associated with an instance
- All instances access the same value

Static Method
- Perform action not tied to an instance
- Can only access static members

Static import statement
- Allows static methods to be used without being class-qualified

Static initialization blocks
- Perform one-time type initialization
- executes before type's first use

Chapter 11 A Closer Look at Methods

Objects are passed by-reference
- Reference is copied to the method

Method changes to the reference
- Not visible outside of the method

Method changes to referenced object
- remain visible outside of the method

Overloading
- Multiple versions of a method or constructor within a class
- Each must have a unique signature

Parts of the signature
- Method name
- Number of parameters
- Type of each parameter

Object class
- Root class of the Java class hierarchy
- Object reference can reference an instance of any class
- Every class has Object characteristics
