# Learn C#

### **C Sharp Introduction**

C# (pronounced as "C sharp") is a modern, object-oriented programming language developed by Microsoft as part of the .NET ecosystem. It is designed to be simple, versatile, and powerful, making it ideal for building a wide range of applications, including web, desktop, mobile, and cloud-based solutions.

---

### **Installing Visual Studio IDE**

**Visual Studio** is an Integrated Development Environment (IDE) developed by Microsoft for creating applications in various programming languages, including C#. You can download and install it from [Visual Studio's website](https://visualstudio.microsoft.com/). During installation, select the **.NET Desktop Development** workload for C# development. This installs all necessary tools for building and debugging C# programs.

---

### **About C#**

C# is part of the .NET framework and runs on the Common Language Runtime (CLR). It’s known for its simplicity, strong type-checking, and object-oriented features, which makes it an ideal language for creating both small and large-scale applications.

---

### **What is .NET Framework?**

The **.NET Framework** is a software development platform developed by Microsoft. It provides a large class library, known as the **Framework Class Library (FCL)**, and supports language interoperability. The core component of the framework is the **Common Language Runtime (CLR)**, which manages the execution of C# and other .NET languages.

---

### **Architecture of .NET Framework**

The .NET Framework has a layered architecture:

1. **Application Layer**: The programs you write (e.g., C# code).
2. **CLR (Common Language Runtime)**: Manages program execution (memory, threading, garbage collection).
3. **FCL (Framework Class Library)**: Provides a set of reusable classes, libraries, and APIs.
4. **Languages**: C#, VB.NET, F#, and others can run on the CLR.

---

### **Build Tools**

Build tools in Visual Studio help compile, link, and package C# programs into executable files or libraries. These tools include:

- **MSBuild**: A build platform used to automate the build process.
- **NuGet**: A package manager to manage external libraries and dependencies.
- **Roslyn**: A compiler for C# and Visual Basic.

---

### **Creating a Project in Visual Studio**

To create a new C# project in Visual Studio:
1. Open Visual Studio.
2. Click on "Create a new project."
3. Choose a project template (e.g., Console App, Windows Forms, ASP.NET Core).
4. Select **C#** as the language.
5. Configure your project settings and click **Create**.

---

### **Running Hello World Program**

A basic "Hello World" program in C# looks like this:

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, World!");
    }
}
```

1. **WriteLine()** prints a message and moves the cursor to a new line.
2. **Write()** prints a message without moving the cursor to a new line.

---

### **Printing Statements (Write() vs WriteLine())**

- **`Console.Write()`**: Prints text without moving to a new line.
- **`Console.WriteLine()`**: Prints text and moves to the next line.

Example:

```csharp
Console.Write("Hello ");
Console.WriteLine("World!");
```

Output:

```
Hello World!
```

---

### **Basic Structure of a C# Program**

A basic C# program consists of:
1. **Namespace**: To organize code logically.
2. **Class**: Defines the blueprint for objects.
3. **Main() Method**: The entry point of the application.

```csharp
namespace HelloWorld
{
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

---

### **What is a Namespace?**

A **namespace** in C# is a container for classes and other types. It helps in organizing code and preventing name conflicts.

```csharp
namespace MyApplication
{
    class MyClass
    {
        // Code goes here
    }
}
```

---

### **Class & Main() Function**

- **Class**: A class is a blueprint for creating objects. It contains methods, properties, and data.
- **Main() Function**: This is the entry point of the program. When you run the program, the code inside `Main()` is executed.

```csharp
class Program
{
    static void Main()
    {
        // Program execution starts here
    }
}
```

---

### **Comments**

- **Single-line comments**: Use `//` to comment a single line of code.
  
  ```csharp
  // This is a comment
  ```

- **Multi-line comments**: Use `/* ... */` for multiple lines.
  
  ```csharp
  /* This is a 
     multi-line comment */
  ```

---

### **Variables**

Variables are used to store data. In C#, you need to declare a variable with a specific type before using it.

```csharp
int age = 25;
string name = "John";
```

---

### **DataTypes**

Common data types in C#:

- **int**: Integer (whole number).
- **float**: Floating-point number (single precision).
- **double**: Floating-point number (double precision).
- **char**: Single character.
- **string**: Sequence of characters (text).
- **bool**: Boolean value (true or false).

---

### **Taking Inputs**

You can take user input using `Console.ReadLine()`.

```csharp
Console.Write("Enter your name: ");
string name = Console.ReadLine();
```

---

### **Size of Datatypes**

The size of some common data types:

- `int`: 4 bytes
- `float`: 4 bytes
- `double`: 8 bytes
- `char`: 2 bytes
- `bool`: 1 byte

---

### **Typecasting Double to Float**

You can convert a `double` to a `float` (explicit casting):

```csharp
double a = 10.5;
float b = (float)a;
```

---

### **Character and Strings**

- **char**: A single character, e.g., `'A'`.
- **string**: A sequence of characters, e.g., `"Hello"`.

---

### **Typecasting Other Datatypes**

You can use explicit or implicit casting for different data types.

```csharp
int i = 10;
double d = i; // Implicit casting
```

For explicit casting:

```csharp
double d = 9.7;
int i = (int)d; // Explicit casting
```

---

### **Taking User Input**

You can take input from the user and convert it to specific types.

```csharp
Console.Write("Enter a number: ");
int num = Convert.ToInt32(Console.ReadLine());
```

---

### **Arithmetic Operators**

Common arithmetic operators:

- `+` (addition)
- `-` (subtraction)
- `*` (multiplication)
- `/` (division)
- `%` (modulus)

Example:

```csharp
int a = 10, b = 5;
int sum = a + b;
```

---

### **Assignment Operators**

Assignment operators assign values to variables:

- `=` (simple assignment)
- `+=`, `-=`, `*=`, `/=`, etc. (compound assignment)

Example:

```csharp
int x = 10;
x += 5; // x = x + 5
```

---

### **Logical Operators**

Logical operators for boolean logic:

- `&&` (AND)
- `||` (OR)
- `!` (NOT)

Example:

```csharp
bool result = (5 > 3) && (2 < 5); // True
```

---

### **Comparison Operators**

Comparison operators are used to compare two values:

- `==` (equal to)
- `!=` (not equal to)
- `<` (less than)
- `>` (greater than)
- `<=` (less than or equal to)
- `>=` (greater than or equal to)

Example:

```csharp
int x = 5;
if (x == 5)
{
    Console.WriteLine("Equal");
}
```

---

### **Math Class in C#**

The **Math** class provides static methods for mathematical operations like absolute value, power, square root, etc.

```csharp
double result = Math.Sqrt(16); // 4
```

---

### **String Methods**

Common string methods:

- `Length`: Returns the length of the string.
- `ToUpper()`: Converts to uppercase.
- `ToLower()`: Converts to lowercase.
- `Substring()`: Extracts a part of the string.

Example:

```csharp
string name = "John";
Console.WriteLine(name.ToUpper()); // JOHN
```

---

### **Escape Sequence Characters**

Escape sequences are special characters used inside strings:

- `\n` (newline)
- `\t` (tab)
- `\\` (backslash)
- `\"` (double quote)

Example:

```csharp
Console.WriteLine("Hello\nWorld");
```

---

### **If Else Statements**

Used for decision-making:

```csharp
int age = 20;
if (age >= 18)
{
    Console.WriteLine("Adult");
}
else
{
    Console.WriteLine("Minor");
}
```

---

### **Loops**

Loops are used for repetitive tasks:

- **for** loop
- **while

** loop
- **do-while** loop

Example:

```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine(i);
}
```

---

### **Methods**

Methods (also called functions) allow you to reuse code.

```csharp
public void Greet()
{
    Console.WriteLine("Hello");
}

static void Main()
{
    Greet(); // Call method
}
```

---

### **Object Oriented Programming in C#**

C# is an object-oriented programming language, which means it focuses on creating objects (instances of classes). It supports key OOP principles:

- **Encapsulation**: Keeping fields private and providing public methods.
- **Inheritance**: Reusing code from other classes.
- **Polymorphism**: Allowing methods to have different behaviors.
- **Abstraction**: Hiding complex implementation details.

Example:

```csharp
class Animal
{
    public void Speak()
    {
        Console.WriteLine("Animal speaks");
    }
}

class Dog : Animal
{
    public void Speak()
    {
        Console.WriteLine("Bark");
    }
}
```

---

This is a broad overview of C# programming concepts, and there’s a lot more to explore as you deepen your understanding of the language.
