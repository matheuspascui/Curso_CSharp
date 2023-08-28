## Program Scope

The Scope Order of a C# Program is, as follows, considering the more important on top:
- importing
- namespace (logical separation)
- Program Class
-Main Method of the program

## Namespace

It is a logical division. It **cannot** contain 2 classes with the same name within this namespace.
Namespaces can be reused (they can be present in many files and programs at a time).
**DO NOT** use Spaces or Special Characters on their names.
Their names **ALWAYS** should start with an Uppercase letter.
- Import files  through namespace (using the keyword `using`).

## "Using " keyword

Importations define the libraries that the program will use. To make an import, we use the **keyword `using`**.


## Variables

Variables are something we use to store values. And, as the name says, their value can change, hence the name variables.
When a variable is created, we define it. When we use it, whe initialize it.
Since C# is a strong typed language, we have 2 options:
- declare the **type** of the variable, or
- use the keyword `var` to create the variable

When creating a variable, the **type** ALWAYS comes first. After that comes the variable's name and after, its value.
if no value was defined for that variable, it'll be created with the standard value. (Like a `int` that will be created with the value `0` as standard.)

### Variable's name

- Do **NOT** start with numbers
- The first letter is LOWERCASE
- Do **NOT** use spaces or special characters

#### Keyword `var`

The keyword `var` is used to define a variable and initialize it with some value. The `var` **doen't** need type declaration, BUT it requires a value declaration (which it'll use to understand the type based on the value).
For example:

```C#
var idade; //error
var age = 24;
```
This example shows that when a value it's not assigned to a variable defined by `var`, it throws an error. Whenn we declare a `var age = 24;`, whe declared and assigned a value to the age, so it works!

### Constansts
- Once created, we are obligated to assign a value to them (these values do NOT change)
- They DO NOT work with `var` 
- They are more optimized them variables
- Recommended for frequent use
- Constans are written **UPPERCASE letters** and the words are **separated by "_" (underline)**
- The idea is to look up the code and rapidly identify a Constant
- They use the **keyword `const`** to be identified

```C#
const int IDADE_MINIMA; //correct because it's assigned the value zero
const int IDADE_MAXIMA = 80; //correct, assigning a value to the constant
```

### Keywords

The Keywords of the C# are blocked to be used by the user. VS Code identifies them and throw an error that we're able to see and corret it.

### Comments

In C#, comments are expressed as: 
- Single Line 
- Multiple Line 
-XML Format (for Metadata)

```C#
//this is a single line comment

/*This is a multiple line comment
in C#'
*/

///This is an XML Metadata comment format
```

### Primitive Types

Also called **built-in types**, the primitive types are the basic ones that come with the language and the foundation to build another ones more complex.
They are classified as:
- Simple Types
- Enums
- Structs
- Nullable Types

The ones that are not the simple types, are the COMPLEX TYPES.

Each primitive type has its own capacity. For example, an `int` has a capacity of ~2 billion.

### System

On .NET, everything starts with a basic type, the `system`. Its use is implicit and it is the base of all objects in .NET.

#### The Primitive Types

- Byte :arrow_right: represent a byte. It can be `signed` or `unsigned`. The `sbyte` is the **signed byte** allows values of -128 to 127. And the **unsigned** byte allows values of 0 to 255. Remember that **1 byte = 8 bits**.


- Int :arrow_right: represent integers. There are 3 variations: `short/ushort`, `int/uint`and `long/ulong`. The ones with the u before are the unsigned ones.

short :arrow_right: 16-bit
int :arrow_right: 32-bit -> It is the DEFAULT type for integer numbers.
long :arrow_right: 64-bit

- Float types: there are the `float`, `double` and `decimal`. They do NOT need the signed/unsigned nomenclature because they accept signs by default.

float :arrow_right: 32-bit -> use and f-notation, like `float salario = 3000.50f`
double :arrow_right: 64-bit It is the DEFAULT type for floating point numbers.
decimal :arrow_right: 128-bit -> use m-notation like `decimal salarioAnual = 25.000m`

- Boolean :arrow_right: bool is a 8-bit type, storing only `true` or `false` values. 

- char :arrow_right: char is a 16-bit type that accepts only one character. It MUST be declared using **single quotes ''**.

- String :arrow_right: is a sequence, or list of characters. It MUST be declared using **single quotes**.

- Var :arrow_right: used to replace the type of the variable. It gets the type of the first declared value.

- Object :arrow_right: generic type that receives any value or object. It doesn't autocomplete with intelisense. Avoid using it.

- Nullable Type :arrow_right: used to represent an empty space. **Every type can be receive null value**, but it has to be declared as a Nullable Type. Use an interrogation simble to mark as a nullable type and assign the `value = null`.

- Alias :arrow_right: is a nickname for the types. All types in .NET have alias. (Ex: System.String has the alias `string` used before).

#### Standard Values

Here will be described the built-in types and their standard values, that are the values assigned if the programmer doesn't do this.
- Int, Decimal, Float :arrow_right: `0`
- bool :arrow_right: `false`
- char :arrow_right: `\0`
- string :arrow_right: `""`
