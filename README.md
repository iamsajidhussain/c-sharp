# C#
This repository contains a comprehensive collection of **C# interview questions** to help you prepare for technical interviews. These questions cover a wide range of topics, from basics to advanced concepts, ensuring you're well-prepared for your next interview.

---

## 🚀 Table of Contents

1. [What is Angular and what are its key features?](#1-what-is-angular-and-what-are-its-key-features)


---

## 📘 Introduction

Welcome to the **C# Interview Questions** repository! Whether you're a beginner or an experienced developer, this repository will help you solidify your knowledge of C# and related technologies. 

### What You'll Find Here:
- Questions categorized by topic for easy navigation.
- Comprehensive answers to help you understand concepts better.
- Code examples for practical understanding.

Feel free to contribute to this repository and make it even more valuable for the community!

---
## 🎯 C# Fundamentals
## 1. What is C# and what are its key features?
**C#** (pronounced as "C-Sharp") is a modern, object-oriented, and type-safe programming language developed by Microsoft as part of the .NET platform. It is primarily used for developing applications that run on Windows, web applications, mobile applications, games (using Unity), and more. C# combines the power of C++ with the ease of Visual Basic, offering a robust and developer-friendly environment.

---

### **Key Features of C#:**

1. **Object-Oriented**:
   C# follows all the principles of object-oriented programming (OOP), such as encapsulation, inheritance, and polymorphism. This makes it easy to model real-world problems.

2. **Type Safety**:
   C# ensures that operations on types are checked at compile time, preventing errors like accessing uninitialized variables or incompatible type assignments.

3. **Automatic Memory Management**:
   C# uses a garbage collector (GC) to handle memory allocation and deallocation, freeing developers from manually managing memory.

4. **Rich Library Support**:
   The .NET framework provides an extensive class library that simplifies common programming tasks such as file handling, database operations, and networking.

5. **Platform Independence (via .NET Core/.NET 5+)**:
   With the advent of .NET Core and later .NET (from .NET 5), C# code can now run on multiple platforms, including Windows, macOS, and Linux.

6. **Asynchronous Programming**:
   The `async` and `await` keywords make it easier to implement asynchronous programming for better performance, especially in I/O-bound operations.

7. **Interoperability**:
   C# allows seamless interaction with other languages, such as C++ or COM objects, and can even call unmanaged code when needed.

8. **LINQ (Language-Integrated Query)**:
   C# provides built-in query capabilities to filter, sort, and group data from different data sources like databases, XML, or collections.

9. **Modern Features**:
   C# keeps evolving with modern features like pattern matching, records, nullable reference types, and more, making it a cutting-edge language.

10. **Security**:
    C# provides built-in support for secure coding practices, with features like code access security (CAS) and type safety, reducing vulnerabilities.

---

### Summary for Quick Review:

- **C#:** A modern, object-oriented language by Microsoft.
- **Key Features:** 
  - Object-oriented, type-safe.
  - Automatic memory management (garbage collection).
  - Cross-platform support via .NET.
  - Asynchronous programming (`async/await`).
  - Rich libraries, LINQ, and modern language features.
  - Secure and interoperable.

<br>

## 2. Explain the basic structure of a C# program.
A basic C# program has a simple and organized structure. It consists of a set of components that work together to define the logic and behavior of the application. Here's an example of a basic C# program and an explanation of its components:

---

#### **Example: Basic C# Program**

```csharp
using System; // 1. Namespace declaration

namespace HelloWorldApp // 2. Namespace
{
    class Program // 3. Class
    {
        static void Main(string[] args) // 4. Main method
        {
            Console.WriteLine("Hello, World!"); // 5. Program logic
        }
    }
}
```

---

#### **Components of a C# Program**

1. **Namespace Declaration**:
   - `using System;`
   - The `using` directive specifies namespaces that contain classes and other elements you want to use in your program.
   - In this case, `System` is a namespace that provides essential classes like `Console`.

2. **Namespace**:
   - `namespace HelloWorldApp`
   - A namespace organizes classes, interfaces, and other code elements into a logical group. This prevents name conflicts between elements in large projects.

3. **Class**:
   - `class Program`
   - Classes are the building blocks of C# programs. Every program must have at least one class. The `Program` class here contains the logic for this simple application.

4. **Main Method**:
   - `static void Main(string[] args)`
   - This is the entry point of the C# application. The runtime starts executing the program from this method.
   - **Details**:
     - **`static`**: Indicates the method belongs to the class and not an instance of the class.
     - **`void`**: Means the method does not return a value.
     - **`string[] args`**: An array of strings that can hold command-line arguments.

5. **Program Logic**:
   - `Console.WriteLine("Hello, World!");`
   - This is the actual code that performs the task. In this example, the program prints "Hello, World!" to the console using the `WriteLine` method of the `Console` class.

---

### Additional Notes:

- **Comments**:
  - Use `//` for single-line comments and `/* ... */` for multi-line comments.
  - Example: `// This is a comment`.

- **Compilation and Execution**:
  - C# code is compiled into Intermediate Language (IL) by the compiler and executed by the .NET runtime.

---

### Summary for Quick Review:

- **Basic Structure**:
  1. Namespace declaration (`using System;`).
  2. Namespace to organize code.
  3. Class as the building block.
  4. Main method (`static void Main`) as the program's entry point.
  5. Program logic executed in the Main method.

<br>

## 3. What are the different types of data types available in C#?
In C#, data types define the type of data a variable can hold. C# has a rich set of data types, which can be broadly categorized into the following:

---

### **1. Value Types**
These hold the actual data and are stored in the **stack memory**. Examples include numbers, characters, and structs.

#### **Common Value Types:**

| Data Type     | Description                       | Example          | Size        | Default Value  |
|---------------|-----------------------------------|------------------|-------------|----------------|
| `byte`        | Unsigned integer (0 to 255)      | `byte b = 255;`  | 1 byte      | `0`            |
| `sbyte`       | Signed integer (-128 to 127)     | `sbyte sb = -5;` | 1 byte      | `0`            |
| `short`       | Signed integer (-32,768 to 32,767) | `short s = -10;` | 2 bytes     | `0`            |
| `ushort`      | Unsigned integer (0 to 65,535)   | `ushort us = 50;`| 2 bytes     | `0`            |
| `int`         | Signed integer (-2B to 2B)       | `int i = 100;`   | 4 bytes     | `0`            |
| `uint`        | Unsigned integer (0 to 4B)       | `uint u = 100U;` | 4 bytes     | `0`            |
| `long`        | Signed integer (-9Q to 9Q)       | `long l = 100L;` | 8 bytes     | `0L`           |
| `ulong`       | Unsigned integer (0 to 18Q)      | `ulong ul = 10;` | 8 bytes     | `0`            |
| `float`       | Single-precision float           | `float f = 1.5F;`| 4 bytes     | `0.0F`         |
| `double`      | Double-precision float           | `double d = 3.14;`| 8 bytes    | `0.0`          |
| `decimal`     | High-precision decimal numbers   | `decimal m = 3.14M;`| 16 bytes | `0.0M`         |
| `char`        | A single Unicode character       | `char c = 'A';`  | 2 bytes     | `'\0'`         |
| `bool`        | Boolean (true/false)             | `bool b = true;` | 1 bit       | `false`        |

---

### **2. Reference Types**
These store the address of the data (a reference to memory) and are stored in the **heap memory**.

#### **Common Reference Types:**

| Data Type    | Description                             | Example                   |
|--------------|-----------------------------------------|---------------------------|
| `object`     | Base type for all data types            | `object o = 42;`         |
| `string`     | Immutable sequence of characters        | `string s = "Hello";`    |
| `dynamic`    | Can hold any type (checked at runtime)  | `dynamic d = 100;`       |

---

### **3. Pointer Types (Unsafe Code)**
Pointer types are used to store memory addresses, but they require the `unsafe` keyword. They're rarely used in modern C# programs.

```csharp
unsafe
{
    int x = 10;
    int* ptr = &x; // Pointer to x
}
```

---

### **4. User-Defined Types**
These are types defined by the programmer to represent custom data structures.

#### **Examples:**

- **Structs**: Value types to hold small, lightweight objects.
  ```csharp
  struct Point { public int X; public int Y; }
  ```
- **Classes**: Reference types for larger and more complex objects.
  ```csharp
  class Person { public string Name; }
  ```
- **Enumerations (Enums)**: Define named constants.
  ```csharp
  enum Colors { Red, Green, Blue }
  ```
- **Delegates**: Represent references to methods.
  ```csharp
  delegate void Display(string message);
  ```

---

### **5. Nullable Types**
C# allows value types to be assigned `null` using nullable types.

```csharp
int? num = null; // Nullable integer
if (num.HasValue)
{
    Console.WriteLine(num.Value);
}
```

---

### Summary for Quick Review:

- **Value Types**: Store data directly (e.g., `int`, `float`, `bool`).
- **Reference Types**: Store memory addresses (e.g., `object`, `string`).
- **Pointer Types**: Hold memory addresses (require `unsafe`).
- **User-Defined Types**: Custom types (e.g., `struct`, `class`, `enum`).
- **Nullable Types**: Allow `null` assignment to value types (`int?`).
<br>

## 4. What is the difference between value types and reference types?
In C#, **value types** and **reference types** are two fundamental categories of data types that differ in how they store data and behave in memory. Understanding these differences is crucial for efficient and error-free programming.

---

### **Key Differences Between Value Types and Reference Types**

| Aspect                | Value Types                              | Reference Types                           |
|-----------------------|------------------------------------------|------------------------------------------|
| **Definition**         | Directly hold data values.               | Hold a reference (memory address) to the data. |
| **Memory Location**    | Stored in the **stack** memory.          | Stored in the **heap** memory, with the reference stored in the stack. |
| **Examples**           | `int`, `float`, `bool`, `struct`, `enum`. | `object`, `string`, `class`, `interface`, `dynamic`, arrays. |
| **Data Handling**      | A copy of the data is passed during assignments or method calls. | A reference (memory address) is passed, meaning changes affect the original object. |
| **Default Value**      | Defaults to a zero-equivalent value (`0` for numbers, `false` for `bool`). | Defaults to `null` (no reference). |
| **Performance**        | Faster for small data since stack access is quicker. | Slower due to heap access and garbage collection. |
| **Garbage Collection** | Not managed by garbage collection (stack memory is auto-managed). | Managed by garbage collection in the heap. |

---

### **Example of Value Type Behavior**

```csharp
int x = 10; // x is a value type
int y = x;  // y gets a copy of x's value
y = 20;     // Changing y does not affect x

Console.WriteLine(x); // Output: 10
Console.WriteLine(y); // Output: 20
```

- Here, `x` and `y` are independent because they store separate copies of the value.

---

### **Example of Reference Type Behavior**

```csharp
class MyClass
{
    public int Value;
}

MyClass obj1 = new MyClass { Value = 10 }; // obj1 points to the object in the heap
MyClass obj2 = obj1;                       // obj2 points to the same object
obj2.Value = 20;                           // Modifies the same object

Console.WriteLine(obj1.Value); // Output: 20
Console.WriteLine(obj2.Value); // Output: 20
```

- Here, `obj1` and `obj2` refer to the same object in memory, so changes made through one reference affect the other.

---

### **When to Use Value Types vs. Reference Types**

1. **Value Types**:
   - Use for small and frequently used data, such as numbers, `bool`, or `enum`.
   - When data is immutable (e.g., coordinates in a 2D plane).

2. **Reference Types**:
   - Use for complex objects, like entities in a database or collections.
   - When data needs to be shared or modified by multiple parts of the program.

---

### Summary for Quick Review:

- **Value Types**: Store data directly in the stack. Examples: `int`, `float`, `bool`.
  - Independent copies during assignment.
  - Faster for small, simple data.

- **Reference Types**: Store references to data in the heap. Examples: `object`, `string`, `class`.
  - Changes affect all references to the object.
  - Better for complex or large data structures.
<br>

## 5. What are nullable types in C#?
### **Detailed Answer**

In C#, **nullable types** allow value types (e.g., `int`, `double`, `bool`) to also hold a `null` value, which is otherwise not possible for value types. This feature is especially useful when dealing with databases or scenarios where a value might be undefined or missing.

---

### **Defining Nullable Types**

A nullable type is defined using the `?` operator after the type. For example:
```csharp
int? nullableInt = null; // Nullable integer
```

This makes the `nullableInt` capable of holding:
- A valid integer value (e.g., `42`).
- A `null` value.

---

### **Nullable Types Declaration**

1. **Using `?` (Shorthand):**
   ```csharp
   int? nullableInt = null; // Nullable int
   bool? nullableBool = true; // Nullable bool
   ```

2. **Using `Nullable<T>` (Full Syntax):**
   ```csharp
   Nullable<int> nullableInt = null; // Equivalent to int?
   ```

---

### **Key Features of Nullable Types**

1. **Default Value:**
   The default value of a nullable type is `null`.

2. **Properties:**
   Nullable types have two main properties:
   - `HasValue`: Returns `true` if the nullable type contains a non-null value, otherwise `false`.
   - `Value`: Retrieves the value if it exists; throws an exception if it’s `null`.

   Example:
   ```csharp
   int? number = 10;

   if (number.HasValue)
   {
       Console.WriteLine($"Value: {number.Value}");
   }
   else
   {
       Console.WriteLine("Value is null.");
   }
   ```

3. **Null Coalescing Operator (`??`):**
   Provides a default value when the nullable type is `null`.

   Example:
   ```csharp
   int? number = null;
   int result = number ?? -1; // If number is null, result will be -1.
   Console.WriteLine(result); // Output: -1
   ```

4. **Null-Conditional Operator (`?.`):**
   Safely access members of an object that might be `null`.

   Example:
   ```csharp
   int? number = null;
   Console.WriteLine(number?.ToString()); // Output: null
   ```

---

### **Practical Example**

#### **Scenario: Nullable Type with Database Values**
In a database, columns might have null values. Nullable types make it easy to handle such data in C#.

```csharp
int? age = GetNullableAgeFromDatabase();

if (age.HasValue)
{
    Console.WriteLine($"Age is {age.Value}");
}
else
{
    Console.WriteLine("Age is not available");
}

int GetNullableAgeFromDatabase()
{
    // Simulating a database return value
    return null; // Can also return an integer value
}
```

---

### **Comparison with Non-Nullable Types**

| Feature               | Non-Nullable Type (`int`) | Nullable Type (`int?`) |
|-----------------------|---------------------------|-------------------------|
| Default Value         | `0`                      | `null`                 |
| Null Assignment       | Not allowed              | Allowed                |
| Properties (`HasValue`, `Value`) | Not applicable           | Available              |

---

### Summary for Quick Review:

- **Nullable Types**: Allow value types to hold `null` values, declared as `int?` or `Nullable<int>`.
- **Key Properties**: 
  - `HasValue`: Checks if a value exists.
  - `Value`: Retrieves the value (throws an exception if `null`).
- **Useful Operators**:
  - `??`: Provides a default value when `null`.
  - `?.`: Safely access members.
- **Common Use**: Handling database or optional values that might be `null`.
<br>

## 6. Can you describe what namespaces are and how they are used in C#?
### **Detailed Answer**

In C#, a **namespace** is a way to organize and group related classes, interfaces, structs, enums, and delegates into a hierarchical structure. It helps avoid naming conflicts, makes code more readable, and provides a logical structure to your application.

---

### **Defining a Namespace**

Namespaces are declared using the `namespace` keyword:

```csharp
namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

In this example:
- `MyApplication` is the namespace.
- The `Program` class is defined within this namespace.

---

### **Purpose of Namespaces**

1. **Avoid Naming Conflicts**:
   - Namespaces allow developers to use the same class name in different parts of the application or libraries without conflicts.
   ```csharp
   namespace LibraryA
   {
       class Math { /* Implementation */ }
   }

   namespace LibraryB
   {
       class Math { /* Different Implementation */ }
   }
   ```

2. **Organize Code**:
   - By grouping related types logically, namespaces make the codebase easier to navigate and maintain.

3. **Provide Scope**:
   - Namespaces define a scope for the identifiers they contain. This ensures that you can reuse class names in different namespaces without clashes.

---

### **Using Namespaces**

1. **Referencing a Namespace**:
   Use the `using` keyword to access members of a namespace:
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

   Here, the `System` namespace is imported, which contains the `Console` class.

2. **Fully Qualified Names**:
   If you don't use the `using` directive, you must use the full path to access a member:
   ```csharp
   class Program
   {
       static void Main()
       {
           System.Console.WriteLine("Hello, World!");
       }
   }
   ```

3. **Nested Namespaces**:
   A namespace can contain other namespaces:
   ```csharp
   namespace OuterNamespace
   {
       namespace InnerNamespace
       {
           class MyClass
           {
               public void Display()
               {
                   Console.WriteLine("Nested Namespace Example");
               }
           }
       }
   }

   class Program
   {
       static void Main()
       {
           var obj = new OuterNamespace.InnerNamespace.MyClass();
           obj.Display();
       }
   }
   ```

---

### **Built-in Namespaces in C#**

C# comes with a rich set of predefined namespaces. Some commonly used ones include:

| Namespace      | Description                                    |
|----------------|------------------------------------------------|
| `System`       | Core types like `Console`, `String`, `Math`.   |
| `System.IO`    | Classes for file and stream handling.          |
| `System.Net`   | Networking-related classes.                   |
| `System.Linq`  | LINQ functionality for querying collections.  |
| `System.Text`  | Classes for handling text and string operations. |
| `System.Threading` | Classes for multi-threading and tasks.       |

---

### **Aliases in Namespaces**

You can create an alias for a namespace to simplify usage:
```csharp
using IO = System.IO;

class Program
{
    static void Main()
    {
        IO.File.WriteAllText("example.txt", "Hello, World!");
    }
}
```

---

### **Real-World Example**

Imagine you are building an application with separate modules for User Management and Products. Namespaces help organize these modules:
```csharp
namespace MyApp.UserManagement
{
    public class User
    {
        public string Name { get; set; }
    }
}

namespace MyApp.Products
{
    public class Product
    {
        public string Name { get; set; }
    }
}
```

Usage:
```csharp
using MyApp.UserManagement;
using MyApp.Products;

class Program
{
    static void Main()
    {
        User user = new User { Name = "Alice" };
        Product product = new Product { Name = "Laptop" };

        Console.WriteLine($"User: {user.Name}, Product: {product.Name}");
    }
}
```

---

### Summary for Quick Review:

- **Namespace**: A container for organizing related types (classes, interfaces, etc.).
- **Purpose**:
  - Avoid naming conflicts.
  - Organize code logically.
  - Define scopes for identifiers.
- **Usage**:
  - Use `using` to import a namespace.
  - Use fully qualified names when necessary.
  - Support for nested namespaces and aliases.
- **Examples**: Common namespaces include `System`, `System.IO`, and `System.Linq`.

Namespaces help keep your code organized and scalable, especially in large applications!
<br>

## 7. Explain the concept of boxing and unboxing in C#.
In C#, **boxing** and **unboxing** are processes used to convert value types and reference types back and forth. These concepts are fundamental to the type system in C# and play a significant role in scenarios involving type conversion.

---

### **What is Boxing?**

**Boxing** is the process of converting a value type (e.g., `int`, `float`, `bool`) into a reference type (specifically, an `object` or any interface type it implements). 

When a value type is boxed:
1. The runtime allocates a new object on the heap.
2. The value is copied from the stack to the heap.
3. A reference to the heap object is returned.

#### **Example of Boxing:**
```csharp
int number = 42; // Value type
object boxedNumber = number; // Boxing

Console.WriteLine(boxedNumber); // Output: 42
```

In this example:
- `number` is a value type stored on the stack.
- `boxedNumber` is a reference type stored on the heap.

---

### **What is Unboxing?**

**Unboxing** is the reverse process of boxing. It converts a reference type (boxed object) back into a value type.

When unboxing:
1. The runtime checks the object’s type to ensure it is the correct value type.
2. The value is copied from the heap back to the stack.

#### **Example of Unboxing:**
```csharp
object boxedNumber = 42; // Boxing
int number = (int)boxedNumber; // Unboxing

Console.WriteLine(number); // Output: 42
```

In this example:
- The boxed object (`boxedNumber`) is cast back to the value type `int`.

---

### **Important Points about Boxing and Unboxing**

1. **Boxing:**
   - Implicit operation (no explicit cast required).
   - Converts value types into reference types.
   - Allocates memory on the heap.

2. **Unboxing:**
   - Explicit operation (requires a cast).
   - Converts a boxed reference type back into a value type.
   - Throws an `InvalidCastException` if the cast fails.

#### **Incorrect Unboxing Example:**
```csharp
object boxedNumber = 42;
double unboxedValue = (double)boxedNumber; // Throws InvalidCastException
```

---

### **Performance Considerations**

- **Boxing and unboxing are costly operations** because:
  1. Boxing involves heap allocation and copying the value.
  2. Unboxing involves type checking and copying the value back to the stack.
- Repeated boxing/unboxing can degrade performance in performance-critical applications.

---

### **Best Practices to Avoid Boxing/Unboxing Overhead**

1. Use **generics** where possible, as they eliminate the need for boxing/unboxing.
   ```csharp
   List<int> numbers = new List<int>(); // No boxing required
   numbers.Add(42);
   ```

2. Avoid storing value types in non-generic collections (e.g., `ArrayList`):
   ```csharp
   ArrayList list = new ArrayList();
   list.Add(42); // Boxing occurs

   int value = (int)list[0]; // Unboxing occurs
   ```

   Use generic collections like `List<T>` instead.

---

### **Real-World Scenario**

#### **Scenario: Using Object with Value Types**
```csharp
void Display(object value)
{
    Console.WriteLine($"Value: {value}");
}

int number = 42;
Display(number); // Boxing occurs when passing the value type
```

Here, the `int` value is boxed into an object to match the `object` parameter type.

---

### **Summary for Quick Review**

- **Boxing**: Converts a value type to a reference type (e.g., `int` → `object`).
  - Implicit.
  - Allocates memory on the heap.
- **Unboxing**: Converts a boxed reference type back to a value type (e.g., `object` → `int`).
  - Explicit (requires a cast).
  - Can throw `InvalidCastException` if the type does not match.
- **Performance**: Avoid unnecessary boxing/unboxing by using generics or appropriate data structures.
- **Example**:
  ```csharp
  int number = 42; // Value type
  object boxed = number; // Boxing
  int unboxed = (int)boxed; // Unboxing
  ```

<br>

## 8. What is Type Casting and what are its types in C#?
### **Detailed Answer**

**Type casting** in C# is the process of converting a value of one data type into another. This is often required when working with different data types or APIs that expect specific types. C# provides two primary types of casting:

1. **Implicit Casting** (safe and automatic conversion).
2. **Explicit Casting** (manual conversion with potential data loss or errors).

---

### **1. Implicit Casting**

- **Definition**: The conversion of a smaller data type to a larger one automatically by the compiler. 
- **Why it's safe**: There is no risk of data loss because the larger type can accommodate the smaller type's value.

#### **Examples of Implicit Casting:**
```csharp
int num = 42;
double result = num; // Implicit casting from int to double

Console.WriteLine(result); // Output: 42.0
```

#### **Supported Conversions for Implicit Casting:**
- From smaller numeric types to larger types (e.g., `int` → `long`, `float` → `double`).
- From derived types to base types (e.g., `Cat` → `Animal`).

---

### **2. Explicit Casting**

- **Definition**: The manual conversion of a larger data type to a smaller one. The programmer must specify the target type using a cast operator (`(type)`).
- **Why it's risky**: It can lead to data loss or runtime errors if the conversion is not valid.

#### **Examples of Explicit Casting:**
```csharp
double num = 42.7;
int result = (int)num; // Explicit casting from double to int

Console.WriteLine(result); // Output: 42 (fractional part is truncated)
```

#### **Unsupported Conversions:**
Attempting to cast incompatible types without conversion logic will result in a runtime error:
```csharp
object obj = "Hello";
int num = (int)obj; // InvalidCastException at runtime
```

---

### **Other Types of Casting in C#**

1. **Type Conversion using Methods**
   - Use built-in methods like `Convert.ToInt32`, `ToString`, etc., for type conversion.
   ```csharp
   string value = "42";
   int result = Convert.ToInt32(value);
   Console.WriteLine(result); // Output: 42
   ```

2. **Using `as` Operator**
   - Performs safe casting of reference types or nullable types. If the cast is invalid, it returns `null` instead of throwing an exception.
   ```csharp
   object obj = "Hello";
   string str = obj as string;

   if (str != null)
       Console.WriteLine("Casting succeeded");
   else
       Console.WriteLine("Casting failed");
   ```

3. **Using `is` Operator**
   - Checks if an object is of a particular type and allows pattern matching.
   ```csharp
   object obj = "Hello";

   if (obj is string str)
       Console.WriteLine($"String: {str}");
   else
       Console.WriteLine("Not a string");
   ```

4. **Boxing and Unboxing**
   - Boxing is implicit casting from a value type to a reference type.
   - Unboxing is explicit casting from a reference type back to a value type.
   ```csharp
   int num = 42;
   object boxed = num; // Boxing
   int unboxed = (int)boxed; // Unboxing
   ```

5. **Custom Conversion Operators**
   - You can define custom implicit and explicit conversion operators in your class.
   ```csharp
   public class Fahrenheit
   {
       public double Degrees { get; set; }
       public static implicit operator Celsius(Fahrenheit f) => new Celsius { Degrees = (f.Degrees - 32) * 5 / 9 };
   }

   public class Celsius
   {
       public double Degrees { get; set; }
   }
   ```

---

### **Key Differences Between Implicit and Explicit Casting**

| Feature               | Implicit Casting           | Explicit Casting           |
|-----------------------|---------------------------|----------------------------|
| **Direction**          | Smaller → Larger          | Larger → Smaller           |
| **Syntax**             | Automatic by the compiler | Requires cast operator      |
| **Risk**               | Safe (no data loss)       | Risk of data loss/errors    |
| **Example**            | `int → long`              | `double → int`             |

---

### **When to Use Each Type**

1. **Use Implicit Casting**:
   - When there is no risk of data loss.
   - For widening conversions like `int` to `long`, `float` to `double`.

2. **Use Explicit Casting**:
   - When narrowing conversions are needed, such as `double` to `int`.
   - When converting between incompatible types with proper checks.

---

### **Summary for Quick Review**

- **Type Casting**: Converts one data type into another.
- **Implicit Casting**: Automatic, safe, no data loss.
  - Example: `int num = 42; double result = num;`
- **Explicit Casting**: Manual, risky, may lose data.
  - Example: `double num = 42.7; int result = (int)num;`
- Other casting methods:
  - `as` for safe reference casting.
  - `is` for type checking and pattern matching.
  - Methods like `Convert.ToInt32` for conversions.
- Use **generics** or proper type-checking to avoid runtime errors.

<br>

## 9. What are operators in C# and can you provide examples?
### **Detailed Answer**

In C#, **operators** are special symbols that perform operations on variables and values. They allow you to manipulate data and control the flow of your program by performing tasks like arithmetic, comparison, logical operations, and more.

### **Types of Operators in C#**

1. **Arithmetic Operators**
2. **Comparison Operators**
3. **Logical Operators**
4. **Assignment Operators**
5. **Unary Operators**
6. **Bitwise Operators**
7. **Conditional Operators**
8. **Null-Coalescing Operators**
9. **Type-Casting Operators**

---

### **1. Arithmetic Operators**

These operators perform basic mathematical operations.

| Operator | Description      | Example            |
|----------|------------------|--------------------|
| `+`      | Addition         | `5 + 3` → `8`      |
| `-`      | Subtraction      | `5 - 3` → `2`      |
| `*`      | Multiplication   | `5 * 3` → `15`     |
| `/`      | Division         | `5 / 3` → `1`      |
| `%`      | Modulus (Remainder) | `5 % 3` → `2`      |

#### **Example:**
```csharp
int a = 5, b = 3;
int sum = a + b;      // sum = 8
int remainder = a % b; // remainder = 2
```

---

### **2. Comparison Operators**

These operators are used to compare two values. They return a boolean value (`true` or `false`).

| Operator | Description      | Example            |
|----------|------------------|--------------------|
| `==`     | Equal to         | `5 == 3` → `false` |
| `!=`     | Not equal to     | `5 != 3` → `true`  |
| `>`      | Greater than     | `5 > 3` → `true`   |
| `<`      | Less than        | `5 < 3` → `false`  |
| `>=`     | Greater than or equal to | `5 >= 3` → `true` |
| `<=`     | Less than or equal to | `5 <= 3` → `false` |

#### **Example:**
```csharp
int a = 5, b = 3;
bool isEqual = (a == b);  // isEqual = false
bool isGreaterThan = (a > b);  // isGreaterThan = true
```

---

### **3. Logical Operators**

Logical operators are used to perform logical operations on boolean values.

| Operator | Description      | Example                |
|----------|------------------|------------------------|
| `&&`     | Logical AND      | `true && false` → `false` |
| `||`     | Logical OR       | `true || false` → `true`  |
| `!`      | Logical NOT      | `!true` → `false`        |

#### **Example:**
```csharp
bool x = true, y = false;
bool andResult = x && y;  // andResult = false
bool orResult = x || y;   // orResult = true
bool notResult = !x;      // notResult = false
```

---

### **4. Assignment Operators**

Assignment operators are used to assign values to variables. 

| Operator | Description      | Example                |
|----------|------------------|------------------------|
| `=`      | Simple assignment| `a = 5`                |
| `+=`     | Add and assign   | `a += 5` → `a = a + 5` |
| `-=`     | Subtract and assign | `a -= 5` → `a = a - 5` |
| `*=`     | Multiply and assign | `a *= 5` → `a = a * 5` |
| `/=`     | Divide and assign | `a /= 5` → `a = a / 5` |
| `%=`     | Modulus and assign | `a %= 5` → `a = a % 5` |

#### **Example:**
```csharp
int a = 10;
a += 5;  // a = 15
a *= 2;  // a = 30
```

---

### **5. Unary Operators**

Unary operators operate on a single operand.

| Operator | Description         | Example            |
|----------|---------------------|--------------------|
| `++`     | Increment (prefix/postfix) | `++a` or `a++`    |
| `--`     | Decrement (prefix/postfix) | `--a` or `a--`    |
| `+`      | Unary plus          | `+a`               |
| `-`      | Unary minus         | `-a`               |
| `!`      | Logical NOT         | `!true` → `false`  |

#### **Example:**
```csharp
int a = 5;
a++;  // a = 6 (Postfix increment)
++a;  // a = 7 (Prefix increment)
```

---

### **6. Bitwise Operators**

Bitwise operators are used to perform bit-level operations.

| Operator | Description           | Example          |
|----------|-----------------------|------------------|
| `&`      | Bitwise AND           | `5 & 3` → `1`    |
| `|`      | Bitwise OR            | `5 | 3` → `7`    |
| `^`      | Bitwise XOR           | `5 ^ 3` → `6`    |
| `~`      | Bitwise NOT (complement) | `~5` → `-6`    |
| `<<`     | Left shift            | `5 << 1` → `10`  |
| `>>`     | Right shift           | `5 >> 1` → `2`   |

#### **Example:**
```csharp
int a = 5, b = 3;
int andResult = a & b;   // andResult = 1
int orResult = a | b;    // orResult = 7
```

---

### **7. Conditional Operator (Ternary Operator)**

The conditional operator is a shorthand for `if-else` statements.

| Operator | Description | Example                           |
|----------|-------------|-----------------------------------|
| `? :`    | Conditional  | `condition ? value_if_true : value_if_false;` |

#### **Example:**
```csharp
int a = 5, b = 3;
int result = (a > b) ? a : b;  // result = 5
```

---

### **8. Null-Coalescing Operators**

These operators are used to simplify null checking.

| Operator | Description            | Example                       |
|----------|------------------------|-------------------------------|
| `??`     | Null-coalescing operator | `var result = value ?? defaultValue;` |

#### **Example:**
```csharp
string value = null;
string result = value ?? "Default";  // result = "Default"
```

---

### **9. Type-Casting Operators**

These operators are used to convert between different types.

| Operator | Description       | Example             |
|----------|-------------------|---------------------|
| `(type)` | Type-casting      | `(int) 42.7` → `42` |

#### **Example:**
```csharp
double a = 42.7;
int b = (int)a;  // b = 42 (casting from double to int)
```

---

### **Summary for Quick Review**

- **Arithmetic Operators**: Perform math operations (`+`, `-`, `*`, `/`, `%`).
- **Comparison Operators**: Compare values (`==`, `!=`, `>`, `<`, `>=`, `<=`).
- **Logical Operators**: Perform logical operations (`&&`, `||`, `!`).
- **Assignment Operators**: Assign values (`=`, `+=`, `-=`, `*=`, `/=`, `%=`).
- **Unary Operators**: Operate on a single operand (`++`, `--`, `+`, `-`, `!`).
- **Bitwise Operators**: Perform operations at the bit level (`&`, `|`, `^`, `~`, `<<`, `>>`).
- **Conditional Operator**: Shorthand for `if-else` (`? :`).
- **Null-Coalescing Operators**: Handle null values (`??`).
- **Type-Casting Operators**: Convert between types (`(type)`).

Would you like more examples or explanations on any specific operator? 😊
<br>

## 10. What is the difference between == operator and .Equals() method?
In C#, both the `==` operator and the `.Equals()` method are used for comparing values, but they work in different ways depending on the context (i.e., value types vs. reference types).

### **1. The `==` Operator**

- The `==` operator is used to compare **values** or **references** depending on whether the types involved are value types or reference types.
- For **value types** (like `int`, `float`, etc.), the `==` operator compares the **actual values**.
- For **reference types** (like `string`, `class` objects), the `==` operator compares **references** (memory addresses), meaning it checks whether both operands point to the same object in memory.

#### **Example with Value Type (int)**
```csharp
int x = 5, y = 5;
bool result = (x == y);  // result = true (compares values)
```

#### **Example with Reference Type (string)**
```csharp
string a = "hello", b = "hello";
bool result = (a == b);  // result = true (compares values, not references)
```

---

### **2. The `.Equals()` Method**

- The `.Equals()` method is a **method** defined in the `System.Object` class, which is the base class of all types in C#.
- By default, `.Equals()` behaves like the `==` operator for **value types** (i.e., it compares the actual values).
- For **reference types**, `.Equals()` is used to compare the **values** inside the objects (e.g., for strings, it compares the characters inside).
- It can be **overridden** in custom classes to implement specific comparison logic based on object content, not just reference or default value comparison.

#### **Example with Value Type (int)**
```csharp
int x = 5, y = 5;
bool result = x.Equals(y);  // result = true (compares values)
```

#### **Example with Reference Type (string)**
```csharp
string a = "hello", b = "hello";
bool result = a.Equals(b);  // result = true (compares values, not references)
```

#### **Example with Custom Class**
```csharp
class Person
{
    public string Name { get; set; }

    public override bool Equals(object obj)
    {
        if (obj == null || this.GetType() != obj.GetType())
            return false;

        Person other = (Person)obj;
        return this.Name == other.Name;
    }
}

Person p1 = new Person() { Name = "John" };
Person p2 = new Person() { Name = "John" };
bool result = p1.Equals(p2);  // result = true (compares Name property)
```

---

### **Key Differences**

| Feature               | `==` Operator                             | `.Equals()` Method                          |
|-----------------------|-------------------------------------------|--------------------------------------------|
| **Default Behavior**   | Compares values for **value types** and references for **reference types**. | Compares values for **value types** and values or reference for **reference types**. |
| **Reference Types**    | Compares memory addresses (references) by default, but for some types like `string`, it compares values. | Compares the content of objects (can be overridden to define custom comparison logic). |
| **Custom Comparison**  | Cannot be customized directly (except through operator overloading). | Can be overridden in custom classes to provide custom equality logic. |
| **Null Comparison**    | Can cause a `NullReferenceException` if comparing a reference type with `null` on the left side (unless the type overloads the operator). | Handles `null` checks properly (you can override `.Equals()` to handle null). |

---

### **Summary for Quick Review**

- **`==` Operator**: Compares values for value types and compares references for reference types.
- **`.Equals()` Method**: Compares values (or custom content) for reference types and value types, and it can be overridden for custom comparison logic.

Would you like more examples or any clarification on these comparisons?
<br>

## 11. What is the purpose of the var keyword in C#?
The `var` keyword in C# is used for **implicitly typed local variables**. This means that the type of the variable is **inferred** by the compiler based on the assigned value, rather than explicitly specifying it. 

### **Key Points About `var`:**

1. **Type Inference**: 
   - When you declare a variable using `var`, the compiler looks at the **right-hand side** (the assigned value) to infer the type of the variable. This can make the code cleaner and more concise.
   - The compiler determines the type at compile-time, and this type cannot change once inferred.

2. **Restrictions**:
   - You **must** assign an initial value when using `var`. Without an initializer, the compiler won’t know what type the variable should be.
   - The type inferred by the compiler cannot be `null` because the compiler won’t be able to determine the type from `null`.

3. **Compile-time Type**:
   - Even though the type is inferred, it is still statically determined at compile-time. The variable behaves just like any other variable of the inferred type.
   
4. **Readability Consideration**:
   - Using `var` can improve readability, especially when the type is obvious from the context or when the type name is long or complex. However, overuse or unclear contexts can reduce readability.

---

### **Example of Using `var`:**

```csharp
// Inferred as int
var number = 5; 

// Inferred as string
var name = "Alice";

// Inferred as List<int>
var numbers = new List<int> { 1, 2, 3, 4 };

// Inferred as a complex object
var person = new Person { Name = "John", Age = 30 };
```

In each case, the type is inferred based on the value assigned to the variable. The type becomes fixed once the variable is declared.

---

### **What Happens if You Don't Use `var`?**

Without `var`, you'd have to specify the type explicitly:

```csharp
int number = 5;
string name = "Alice";
List<int> numbers = new List<int> { 1, 2, 3, 4 };
```

While this is perfectly fine, `var` makes it more concise, especially in cases where the type is obvious or where you're working with complex types.

---

### **When Not to Use `var`:**

- **When the type is unclear**: If the type isn't obvious from the context, it’s better to specify the type explicitly to make the code more readable.
- **When you want to maintain explicit clarity**: In some situations, you might prefer clarity over brevity, especially when working with more complex data structures.

---

### **Summary for Quick Review**

- **Purpose**: `var` allows for **implicit typing** where the compiler determines the variable's type based on the assigned value.
- **When to Use**: When the type is obvious from the assigned value or to make code cleaner and more concise.
- **When Not to Use**: When the type is unclear or when you want to be explicit for readability.

<br>

## 12. What are the differences between const and readonly keywords?
### **Detailed Answer**

In C#, both `const` and `readonly` are used to define variables with values that **cannot be modified** after initialization, but they have key differences in their usage and behavior.

### **1. `const` Keyword**

- **Compile-time Constant**: 
  - A `const` variable is **evaluated at compile time**. Its value must be assigned at the time of declaration and cannot be changed after that.
  
- **Usage**:
  - A `const` can only be assigned a **literal value** or an expression that can be evaluated at compile time.
  
- **Scope**:
  - Constants are **implicitly static**, meaning they are shared across all instances of a class or structure. They are not tied to any particular object instance.
  
- **Type**:
  - Constants can only be of a **primitive type** (like `int`, `double`, `char`, etc.), `enum`, or a **string**.
  
- **Access**:
  - Constants are generally used for values that **do not change** throughout the program execution, such as mathematical constants (`PI`, `E`), or fixed configuration values.
  
#### **Example of `const`:**
```csharp
public class MathConstants
{
    public const double Pi = 3.14159;  // Compile-time constant
}

Console.WriteLine(MathConstants.Pi);  // 3.14159
```

---

### **2. `readonly` Keyword**

- **Run-time Constant**:
  - A `readonly` variable can be assigned a value either at **declaration** or in the **constructor** of the class. Its value can only be modified once (during object initialization).
  
- **Usage**:
  - `readonly` is used for values that should be set at runtime but remain unchanged after that (e.g., configuration values initialized during object creation).
  
- **Scope**:
  - `readonly` variables can be instance-specific or static. This means they can be tied to an instance or shared across all instances (if declared static).
  
- **Type**:
  - `readonly` can be of any type, including reference types or more complex objects, not just primitive types.

#### **Example of `readonly`:**
```csharp
public class Circle
{
    public readonly double radius;  // Read-only field

    public Circle(double r)
    {
        radius = r;  // Set value during object creation
    }
}

Circle circle = new Circle(5);
Console.WriteLine(circle.radius);  // 5

// circle.radius = 10;  // Compile-time error: Cannot modify the readonly field 'radius'
```

---

### **Key Differences Between `const` and `readonly`:**

| Feature                    | `const`                                | `readonly`                                  |
|----------------------------|----------------------------------------|---------------------------------------------|
| **Assignment**              | Must be assigned at **declaration**.   | Can be assigned at **declaration** or in the **constructor**. |
| **Value Change**            | Cannot be changed after initialization. | Can only be changed once, either at declaration or in the constructor. |
| **Compile-time vs Runtime** | Evaluated at **compile-time**.         | Evaluated at **runtime**.                   |
| **Type**                    | Can only be primitive types or `string`. | Can be any type, including complex objects or reference types. |
| **Scope**                   | Implicitly **static**, shared across all instances. | Can be **instance-specific** or **static**. |
| **Access**                  | Typically used for constants like mathematical values. | Used for values that should be set at runtime but remain unchanged after that. |

---

### **Summary for Quick Review**

- **`const`**: Must be assigned at compile-time, cannot be changed, and is implicitly static.
- **`readonly`**: Can be assigned at runtime (via constructor), can be instance-specific or static, and can be used with any type.

Would you like more examples or further clarification on this topic?
<br>

## 13. How does checked and unchecked context affect arithmetic operations?
### **Detailed Answer**

In C#, the `checked` and `unchecked` contexts are used to control how **overflow** is handled during arithmetic operations, especially with integral types (like `int`, `short`, `long`, etc.).

### **1. `checked` Context**

- The **`checked`** context ensures that any arithmetic operation that results in an **overflow** will throw an exception.
- Overflow occurs when a value exceeds the maximum or minimum value that a data type can hold. For example, trying to store a value larger than `int.MaxValue` (2,147,483,647) in an `int` will cause an overflow.
- In `checked` context, if such an overflow occurs, a `System.OverflowException` will be thrown.

#### **Example of `checked` context**:
```csharp
try
{
    int a = int.MaxValue;
    int b = 1;
    int result = checked(a + b);  // Throws OverflowException
}
catch (OverflowException ex)
{
    Console.WriteLine("Overflow occurred: " + ex.Message);
}
```
- In the above example, adding `1` to `int.MaxValue` results in an overflow, and because it’s in the `checked` context, an `OverflowException` is thrown.

---

### **2. `unchecked` Context**

- The **`unchecked`** context allows arithmetic operations to **ignore overflow** and **wrap around** the result (i.e., it treats the overflow as if it’s a "modulo" operation).
- By default, C# performs arithmetic operations in the `unchecked` context, so overflow results in the value wrapping around (i.e., it starts again from the minimum value of the type).
  
#### **Example of `unchecked` context**:
```csharp
int a = int.MaxValue;
int b = 1;
int result = unchecked(a + b);  // No exception, result wraps around
Console.WriteLine(result);  // Prints: -2147483648 (overflowed to the minimum value)
```
- In this case, adding `1` to `int.MaxValue` causes the value to overflow and wrap around to `int.MinValue` (`-2147483648`), and no exception is thrown.

---

### **3. Default Context (Unchecked)**

By default, C# performs arithmetic operations in the `unchecked` context, meaning that overflow will **not throw an exception** and the result will wrap around within the bounds of the data type.

#### **Example of Default Behavior**:
```csharp
int a = int.MaxValue;
int b = 1;
int result = a + b;  // No exception, result wraps around
Console.WriteLine(result);  // Prints: -2147483648 (overflowed to the minimum value)
```

---

### **4. Using `checked` and `unchecked` Blocks**

You can apply the `checked` and `unchecked` keywords to entire code blocks, ensuring that all operations within those blocks are handled according to the specified overflow behavior.

#### **Example of `checked` block**:
```csharp
checked
{
    int a = int.MaxValue;
    int b = 1;
    int result = a + b;  // Throws OverflowException
}
```

#### **Example of `unchecked` block**:
```csharp
unchecked
{
    int a = int.MaxValue;
    int b = 1;
    int result = a + b;  // Result wraps around, no exception
    Console.WriteLine(result);  // Prints: -2147483648
}
```

---

### **Key Differences Between `checked` and `unchecked`**

| Feature             | `checked`                                | `unchecked`                               |
|---------------------|------------------------------------------|-------------------------------------------|
| **Overflow Behavior**| Throws `OverflowException` on overflow.  | Ignores overflow and wraps the value around. |
| **Default Context**  | Not the default. Must be explicitly used. | The default context for arithmetic operations. |
| **Use Case**         | Used when you want to detect overflow errors. | Used when overflow handling is not required or you want to avoid exceptions. |

---

### **Summary for Quick Review**

- **`checked`**: Forces overflow to throw an `OverflowException`.
- **`unchecked`**: Allows overflow to wrap around without throwing an exception (default behavior).

This context is particularly useful when dealing with fixed-width integral types where overflow might be a concern, and handling it accordingly is necessary for your application logic.

Would you like more examples or further clarification on this topic?
<br>

## 14. What are the different ways to handle errors in C#?
### **Detailed Answer**

In C#, errors are typically handled using **exception handling** mechanisms. These mechanisms allow your program to detect and handle runtime errors (exceptions) that occur during program execution.

Here are the key ways to handle errors in C#:

---

### **1. Using Try-Catch-Finally**

The **try-catch-finally** block is the most common way to handle exceptions. It allows you to attempt an operation that might fail (in the `try` block), catch any exceptions that occur (in the `catch` block), and finally, run cleanup code (in the `finally` block).

#### **Syntax:**
```csharp
try
{
    // Code that might throw an exception
}
catch (ExceptionType ex)
{
    // Code to handle the exception
}
finally
{
    // Code that runs no matter what (optional)
}
```

#### **Example:**
```csharp
try
{
    int num1 = 10;
    int num2 = 0;
    int result = num1 / num2;  // This will cause a divide-by-zero exception
}
catch (DivideByZeroException ex)
{
    Console.WriteLine("Error: Cannot divide by zero.");
}
finally
{
    Console.WriteLine("This will always run.");
}
```

- In this example, the `catch` block will handle the divide-by-zero error, and the `finally` block will always run, even if an exception occurs.

---

### **2. Using Multiple Catch Blocks**

You can have multiple `catch` blocks to handle different types of exceptions. This allows you to handle specific exceptions in a tailored way.

#### **Syntax:**
```csharp
try
{
    // Code that might throw different types of exceptions
}
catch (Type1Exception ex)
{
    // Handle Type1Exception
}
catch (Type2Exception ex)
{
    // Handle Type2Exception
}
```

#### **Example:**
```csharp
try
{
    int[] numbers = new int[] { 1, 2, 3 };
    Console.WriteLine(numbers[5]);  // This will throw an IndexOutOfRangeException
}
catch (IndexOutOfRangeException ex)
{
    Console.WriteLine("Error: Index out of range.");
}
catch (Exception ex)
{
    Console.WriteLine("General error: " + ex.Message);
}
```

- In this case, the specific `IndexOutOfRangeException` is caught first, and if any other exception occurs, the general `Exception` handler catches it.

---

### **3. Throwing Exceptions (throw)**

You can **throw** exceptions intentionally using the `throw` keyword. This is useful when you want to signal an error in your code or pass an exception from one method to another.

#### **Syntax:**
```csharp
throw new Exception("Error message");
```

#### **Example:**
```csharp
public void ProcessData(int value)
{
    if (value <= 0)
    {
        throw new ArgumentException("Value must be greater than zero.");
    }
}
```

- This method throws an exception if the input `value` is less than or equal to zero.

---

### **4. Custom Exceptions**

You can create custom exception classes by inheriting from the base `Exception` class. This allows you to create specific exception types suited to your application.

#### **Example:**
```csharp
public class InvalidAgeException : Exception
{
    public InvalidAgeException() : base("Age is not valid.") { }
    public InvalidAgeException(string message) : base(message) { }
}
```

- This custom exception class can be used to throw and catch specific errors related to age validation in your application.

---

### **5. Using Exception Filters (C# 6 and later)**

Starting with C# 6, you can use **exception filters** to apply additional conditions to the `catch` block. This allows you to handle exceptions only when specific conditions are met.

#### **Syntax:**
```csharp
try
{
    // Code that might throw an exception
}
catch (ExceptionType ex) when (ex.Property > 0)
{
    // Handle the exception only when a condition is met
}
```

#### **Example:**
```csharp
try
{
    int number = -5;
    if (number < 0) throw new ArgumentOutOfRangeException("number", "Number cannot be negative.");
}
catch (ArgumentOutOfRangeException ex) when (ex.ParamName == "number")
{
    Console.WriteLine("Caught an invalid number argument: " + ex.Message);
}
```

- In this example, the exception is only handled if the parameter name is `"number"`, demonstrating how exception filters work.

---

### **6. Using Loggers to Track Errors**

In addition to handling errors, it's important to log them for later analysis. You can use various **logging frameworks** (such as `Serilog`, `NLog`, or `log4net`) to log exceptions, which is crucial for debugging and production environments.

#### **Example with a Logger:**
```csharp
try
{
    // Code that might throw an exception
}
catch (Exception ex)
{
    Logger.Error(ex, "An error occurred in the application.");
}
```

- This would log the exception message and stack trace using a logger, providing more information for debugging.

---

### **7. Handling Unhandled Exceptions (Global Handling)**

In some cases, exceptions may not be caught locally, and you need to handle them globally. In a **console application**, you can subscribe to `AppDomain.CurrentDomain.UnhandledException` for global error handling. In **ASP.NET** applications, the `Application_Error` event in the `Global.asax` file handles unhandled exceptions globally.

#### **Example (Console Application)**:
```csharp
AppDomain.CurrentDomain.UnhandledException += (sender, args) =>
{
    Console.WriteLine("Unhandled exception: " + args.ExceptionObject.ToString());
};
```

---

### **Summary for Quick Review**

- **Try-Catch-Finally**: Handles errors during code execution.
- **Multiple Catch Blocks**: Handles different types of exceptions.
- **Throwing Exceptions**: Used to throw custom or predefined exceptions.
- **Custom Exceptions**: Define your own exception types by inheriting from `Exception`.
- **Exception Filters**: Handle exceptions conditionally based on specific criteria.
- **Logging**: Use logging frameworks to track exceptions for debugging and production environments.
- **Global Handling**: Handle unhandled exceptions globally using event handlers.

Let me know if you'd like more details or examples on any specific error handling mechanism!
<br>

## 15. Explain the role of the garbage collector in .NET.
### **Detailed Answer**

The **Garbage Collector (GC)** in .NET is a memory management feature that automatically handles the release of memory used by objects that are no longer needed or accessible in your application. The primary role of the garbage collector is to manage the lifecycle of objects in memory and ensure that memory is freed when it's no longer in use, helping to prevent memory leaks and optimize the performance of the application.

---

### **How Garbage Collection Works in .NET:**

1. **Automatic Memory Management:**
   The GC automatically manages memory for objects created on the heap. It removes objects that are no longer reachable, which means no part of your program can access them.

2. **Heap Memory:**
   In .NET, memory is divided into two main areas:
   - **Stack:** This is used for storing local variables and method call information. The memory on the stack is automatically freed when a method completes.
   - **Heap:** This is where objects created using `new` are stored. The GC primarily manages heap memory.

3. **Generations:**
   The .NET garbage collector uses a generation-based approach to optimize performance. Objects are divided into **three generations**:
   - **Generation 0 (Young Generation):** Newly created objects are placed in Generation 0. These objects are typically short-lived and are garbage collected frequently.
   - **Generation 1 (Middle Generation):** If an object survives a GC collection in Generation 0, it is promoted to Generation 1. Objects in this generation are less likely to be garbage collected frequently.
   - **Generation 2 (Old Generation):** Objects that continue to survive garbage collection cycles are promoted to Generation 2. These objects are long-lived, and GC only runs on them occasionally.

4. **Mark-and-Sweep Process:**
   The GC follows a **Mark-and-Sweep** process to identify which objects can be collected:
   - **Marking Phase:** The GC starts by identifying all reachable objects from the root (like global variables, local variables on the stack, and references in static fields). Any object that is accessible is marked as alive.
   - **Sweeping Phase:** After marking, the GC goes through the heap and frees up memory for the objects that are not marked (i.e., objects that are no longer reachable).

5. **Compact and Defragmentation:**
   After sweeping, the GC may compact the heap to reduce fragmentation. It moves surviving objects to one contiguous area in memory, which makes future allocations more efficient.

---

### **Key Responsibilities of the Garbage Collector:**

1. **Memory Management:**
   The garbage collector automatically frees memory that is no longer needed, helping to avoid memory leaks. Without GC, developers would need to manually release memory, which could be error-prone.

2. **Optimizing Memory Usage:**
   By collecting unused objects in different generations and collecting them at different times, the GC helps in optimizing memory usage and minimizing pauses caused by collection.

3. **Reducing Developer Overhead:**
   The GC eliminates the need for manual memory management (like calling `free()` in C or C++), thus reducing the chances of errors like double-freeing memory or leaving memory unreleased.

4. **Automatic Cleanup:**
   The GC also helps in automatically cleaning up resources such as file handles or database connections via the finalization process, although relying on finalizers can slow down the collection process.

---

### **Garbage Collection Events:**

- **Minor GC (Generation 0):** This happens when Generation 0 is full, and objects are promoted to Generation 1. It is usually fast and happens often.
- **Major GC (Generation 1 or 2):** This occurs less frequently but can take longer. It occurs when objects in Generation 1 or 2 are no longer needed.
- **Full GC:** This is a comprehensive garbage collection process that checks all generations, cleans up unreachable objects, and compacts the heap. It can be more expensive in terms of performance.

---

### **When Does Garbage Collection Happen?**

- The GC runs automatically when the system detects low memory or when a certain threshold of memory usage is reached. However, you can also trigger garbage collection manually using `GC.Collect()`, but it's generally not recommended to do so, as the .NET runtime is highly optimized for automatic garbage collection.
  
  #### **Example of triggering GC:**
  ```csharp
  GC.Collect();
  ```

  - Although you can manually trigger GC, doing so too frequently can reduce performance. It's usually better to let the GC run automatically based on its internal optimization.

---

### **Finalization and IDisposable:**

- **Finalizer:** In C#, objects can define a `finalize()` method (called `~ClassName()`), which the garbage collector calls when the object is collected. This is useful for releasing unmanaged resources like file handles, database connections, etc.
  - However, relying on finalization can be slower and less predictable. It's often better to use `IDisposable` for deterministic resource cleanup.

- **IDisposable Interface:** Classes that manage resources (like file streams or database connections) implement the `IDisposable` interface to provide a `Dispose()` method for explicitly freeing resources when they're no longer needed.

#### **Example of implementing IDisposable:**
```csharp
public class ResourceHandler : IDisposable
{
    private bool disposed = false;

    public void Dispose()
    {
        if (!disposed)
        {
            // Release unmanaged resources here
            disposed = true;
            GC.SuppressFinalize(this);
        }
    }

    ~ResourceHandler()
    {
        Dispose();
    }
}
```
- In the example, `Dispose()` is called to release resources, and `GC.SuppressFinalize(this)` ensures that the finalizer is not called if `Dispose()` has already cleaned up resources.

---

### **Summary for Quick Review**

- **Garbage Collector (GC):** Automatically manages memory by cleaning up unused objects from the heap.
- **Generations:** The GC divides objects into Generation 0, 1, and 2 for optimized memory management.
- **Mark-and-Sweep:** The GC identifies and cleans up unreachable objects in the heap.
- **Minor and Major GC:** These refer to garbage collection events that happen at different stages (Generation 0 vs. Generation 1/2).
- **Finalization & IDisposable:** Helps in cleaning up unmanaged resources. Use `IDisposable` and `Dispose()` for deterministic cleanup.
<br>

## 🎯 Object-Oriented Programming in C#
## 16. Define Object-Oriented Programming and its principles.
### **Object-Oriented Programming (OOP)**

**Object-Oriented Programming (OOP)** is a programming paradigm based on the concept of "objects," which can contain data and methods that operate on the data. OOP focuses on organizing software around data (objects) rather than functions and logic. It enables more modular, reusable, and maintainable code.

In OOP, objects are instances of classes, which define their structure (properties) and behavior (methods). It emphasizes the use of abstraction, inheritance, polymorphism, and encapsulation to create more flexible and scalable software.

---

### **Key Principles of Object-Oriented Programming**

There are four core principles of OOP:

#### 1. **Encapsulation**
   - **Definition:** Encapsulation is the concept of bundling the data (properties) and the methods (functions) that operate on the data into a single unit known as a class. It also restricts direct access to some of an object's components, which is why it is often referred to as "data hiding."
   - **Purpose:** It helps protect an object's internal state from unintended modification by outside code and ensures that the object’s data can only be accessed or modified through defined methods.
   - **Example:**
     ```csharp
     public class Person
     {
         private string name;  // Private field
         
         // Public method to access private field
         public string Name
         {
             get { return name; }
             set { name = value; }
         }
     }
     ```
     In the above example, the `name` field is encapsulated within the `Person` class and can only be accessed or modified through the `Name` property.

#### 2. **Abstraction**
   - **Definition:** Abstraction is the process of hiding the complex implementation details and showing only the essential features of the object. It allows a user to interact with an object through simplified interfaces.
   - **Purpose:** It reduces complexity by providing only relevant data and operations to the user, and shields them from the implementation details.
   - **Example:**
     ```csharp
     public abstract class Animal
     {
         public abstract void MakeSound();  // Abstract method
     }

     public class Dog : Animal
     {
         public override void MakeSound()
         {
             Console.WriteLine("Woof");
         }
     }
     ```
     In this example, the `Animal` class is abstract, meaning it provides a general structure but no implementation of `MakeSound()`. The `Dog` class provides the specific implementation for the `MakeSound()` method.

#### 3. **Inheritance**
   - **Definition:** Inheritance allows a class (child class) to inherit the properties and methods from another class (parent class). It helps in reusing the code and creating a hierarchical relationship between classes.
   - **Purpose:** It promotes code reuse and allows for the extension of existing functionality without modifying the original code.
   - **Example:**
     ```csharp
     public class Animal
     {
         public void Eat()
         {
             Console.WriteLine("Eating...");
         }
     }

     public class Dog : Animal  // Dog inherits from Animal
     {
         public void Bark()
         {
             Console.WriteLine("Barking...");
         }
     }

     Dog dog = new Dog();
     dog.Eat();  // Inherited method
     dog.Bark(); // Method of Dog class
     ```
     In the example above, the `Dog` class inherits the `Eat()` method from the `Animal` class and adds its own `Bark()` method.

#### 4. **Polymorphism**
   - **Definition:** Polymorphism allows objects of different classes to be treated as objects of a common superclass. The most common use of polymorphism is when a parent class reference is used to refer to a child class object. It allows the same method to behave differently based on the object it is called on.
   - **Purpose:** Polymorphism provides flexibility in using objects of different types through a common interface and allows for method overriding and overloading.
   - **Types:**
     - **Compile-time polymorphism (Method Overloading):** Occurs when multiple methods have the same name but different parameters.
     - **Run-time polymorphism (Method Overriding):** Occurs when a subclass provides a specific implementation of a method already defined in the superclass.
   - **Example:**
     ```csharp
     public class Animal
     {
         public virtual void MakeSound()
         {
             Console.WriteLine("Some generic animal sound");
         }
     }

     public class Dog : Animal
     {
         public override void MakeSound()
         {
             Console.WriteLine("Bark");
         }
     }

     public class Cat : Animal
     {
         public override void MakeSound()
         {
             Console.WriteLine("Meow");
         }
     }

     Animal myAnimal = new Animal();
     myAnimal.MakeSound();  // Outputs: Some generic animal sound

     Animal myDog = new Dog();
     myDog.MakeSound();  // Outputs: Bark

     Animal myCat = new Cat();
     myCat.MakeSound();  // Outputs: Meow
     ```
     In this example, `MakeSound()` is overridden in both the `Dog` and `Cat` classes. The method behaves differently depending on whether it is called on an `Animal`, `Dog`, or `Cat` object, demonstrating polymorphism.

---

### **Summary for Quick Review**

- **Object-Oriented Programming (OOP):** A programming paradigm based on organizing code into objects that combine data and behavior.
- **Key Principles:**
  1. **Encapsulation:** Bundles data and methods into a class while restricting direct access to the data.
  2. **Abstraction:** Hides complex implementation details and exposes only essential features.
  3. **Inheritance:** Allows a class to inherit properties and methods from another class, promoting code reuse.
  4. **Polymorphism:** Enables a method to behave differently based on the object it is called on, supporting both method overloading and overriding.

These principles work together to make OOP a powerful and flexible paradigm for software design and development.
<br>

## 17. What is a class and how is it different from a struct?

<br>

## 18. Explain the concept of inheritance and its use in C#.

<br>

## 19. What is polymorphism, and can you give a C#_ example?

<br>

## 20. What is encapsulation and how is it implemented in C#?

<br>

## 21. What are abstract classes and interfaces, and when do you use each?

<br>

## 22. Can you explain what a virtual method is in C#?

<br>

## 23. What is method overloading and method overriding?

<br>

## 24. Can you describe the base keyword?

<br>

## 25. What is an access modifier and what are the different types of access modifiers?

<br>

## 🎯 C# Advanced Concepts
## 26. What are indexers in C#?

<br>

## 27. Explain the concept of delegates in C#.

<br>

## 28. What are events and how are they different from delegates?

<br>

## 29. What are Lambda expressions and where would you use them?

<br>

## 30. Can you explain what extension methods are and how to use them?

<br>

## 31. What are generics and how do they provide type safety?

<br>

## 32. Define LINQ and mention its advantages.

<br>

## 33. What is the difference between IEnumerable and IQueryable?

<br>

## 34. What are async and await keywords and how do they work?

<br>

## 35. What is the purpose of the using statement?

<br>

## 🎯 C# Collections and Data Structures
## 36. What are collections in C#?

<br>

## 37. What is the difference between arrays and collections?

<br>

## 38. Explain the different types of collections in .NET.

<br>

## 39. What is the difference between List and LinkedList?

<br>

## 40. Can you discuss the IDictionary interface and its implementation?

<br>

## 41. What are HashTable and Dictionary and how do they differ?

<br>

## 42. How does a C# HashSet work and what are its benefits?

<br>

## 43. What are Enumerable and Queryable collections?

<br>

## 44. When would you use a Queue vs a Stack?

<br>

## 45. How do you sort elements in a collection?

<br>

## 🎯 C# Exception Handling
## 46. What is exception handling and why is it necessary?

<br>

## 47. What are the common exception types in C#?

<br>

## 48. How do you create custom exceptions in C#?

<br>

## 49. What is the use of the finally block?

<br>

## 50. Can you explain exception filters introduced in C# 6?

<br>

## 🎯 C# Asynchronous Programming
## 51. What is the Task Parallel Library (TPL)?

<br>

## 52. Explain the difference between synchronous and asynchronous operations.

<br>

## 53. How do you cancel an asynchronous operation?

<br>

## 54. What is the difference between Task and Thread?

<br>

## 55. Discuss the use of the Parallel class in C#.

<br>

## 🎯 C# File I/O and Serialization
## 56. How do you read from and write to a text file in C#?

<br>

## 57. What are the file handling classes in C#?

<br>

## 58. Explain serialization and deserialization in the context of C#. 

<br>

## 59. What is the difference between XML Serialization and JSON Serialization? 

<br>

## 60. How do you use streams in C#?

<br>

## 🎯 C# Attributes and Reflection 
## 61. What are attributes in C#? 

<br>

## 62. How do you define a custom attribute? 

<br>

## 63. What is reflection and why is it useful? 

<br>

## 64. Explain how to use reflection to inspect an assembly’s metadata. 

<br>

## 65. How do you use reflection to create an instance of a class at runtime?

<br>

## 🎯 C# Memory Management 
## 66. Describe the stack and heap in .NET’s memory management. 

<br>

## 67. What are the finalizers in C#? 

<br>

## 68. How do you force a garbage collection? 

<br>

## 69. Explain the IDisposable interface and the Dispose pattern. 

<br>

## 70. What is a memory leak in .NET and how can it be prevented?

<br>

## 🎯 C# Debugging and Diagnostic 
## 71. How do you debug a C# application? 

<br>

## 72. What are breakpoints and how are they used? 

<br>

## 73. Explain the use of the Debug and Trace classes. 

<br>

## 74. Discuss the techniques to analyze a memory dump.

<br>

## 75. How can you profile a C# application to identify performance bottlenecks?

<br>

## 🎯 C# Concurrency and Parallelism 
## 76. What is a deadlock and how can it be prevented? 

<br>

## 77. Discuss the reader-writer lock pattern in C#. 

<br>

## 78. Explain how the lock keyword ensures thread safety. 

<br>

## 79. What are Mutexes, Semaphores, and Monitors? 

<br>

## 80. How do you achieve parallelism using PLINQ?

<br>

## 🎯 C# Unit Testing and Test Driven Development (TDD) 
## 81. What is unit testing and what frameworks do you use for it in C#? 

<br>

## 82. Explain the concept of Test-Driven Development (TDD). 

<br>

## 83. How do you mock objects in C# unit tests? 

<br>

## 84. What are the common attributes used in a test method?  

<br>

## 85. How do you test asynchronous code in C#?

<br>

## 🎯 C# Best Practices and Design Patterns 
## 86. Why are SOLID principles important in C#?

<br>

## 87. Can you describe some common design patterns and their applications in C#?

<br>

## 88. How do you ensure your C# code is maintainable and readable? 

<br>

## 89. What strategies do you use for error handling and exception management? 

<br>

## 90. Discuss the concept of dependency injection and how it’s used in C#. 

<br>

## 91. What are the new features introduced in the latest version of C#? 

<br>

## 92. How has pattern matching evolved in recent C# versions? 

<br>

## 93. Explain how C#8 nullable reference types work. 

<br>

## 94. What is the switch expression and how does it differ from the switch statement? 

<br>

## 95. How do you take advantage of tuples in C#?

<br>

## 🎯 C# Interoperability 
## 96. How can you call unmanaged code using C#? 

<br>

## 97. What is the role of P/Invoke in C#? 

<br>

## 98. How do you interface with COM objects in C#? 

<br>

## 99. Discuss C# and .NET Core inter-platform capabilities.

<br>

## 100. How is C# evolving with .NET 5 and beyond?

<br>
