# SWI 4

## data types

- data types are ways how we can categorize various types of data and store them in relevant ways into computer memory
- some examples:
	- **int** - whole numbers
		- **short** - 2 bytes
		- **int** - 4 bytes
		- **long** - 8 bytes
	- **double**, **float** - decimal point numbers
	- **char** - text character type
	- **string** - an array of **char** types, used for storing text
	- **boolean** - used for storing true or false statements
	- **array** - used for storing multiple instances of data in one entry
	- **dictionary** - similar to the **array**, but instead of things being identified by order, they are identified by a key-value pair

## variables

- a way how we can store, read and modify values in code
	- a way how id explain a variable is a digital box, where we can put values in it, look whats in it or modify the value in it

## static vs dynamic typing

- with static typing, the variables data type needs to be defined during declaration and cannot be changed after
	- with arrays or dictionaries, their specific data type and size needs to be determined during declaration too
	- this is necessary for many compiled languages (ie. C, C++, C#, Java) as it tells the compiler how much memory the program must allocate
	- some languages (such as C++ or C#) have an `auto` or `var` data type
		- the data type gets defined by the first value that gets written into the variable, this is done by the compiler and is called **implicit typing**
- with dynamic typing, a variable doesnt need to have a defined type
	- arrays and dictionaries allocate as much memory as they need, which leads to them having a non-fixed size and in some languages, a possible mix of different types of data in them
	- dynamic typing is usually seen in interpreted languages such as Python or JavaScript

## declaration

- declaring a variable in code allocates a space in memory needed for storing the given data type
- a declared variable requires a name
- example: `int a;`
- data does not need to be written into the variable in this stage yet!

## initialization

- initialization occurs when data is first inserted into a variable
	- usually happens during declaration, when a variable is declared like this: `int a = 3;`
	- can occur later as well, like this: `int a;` and then `a = 3;`

## references

- another data type exists - the **pointer**
- a pointer allows the user to not pass the value of the variable to a function as an example, but the address to the given variable
	- this allows the function to read it or overwrite it directly instead of working with just the value
- there are also **references**, that are an alternative to pointers
	- they are safer, since they work more as an "alias" instead of an actual direct memory address

## immutability

- a variable can be defined as a constant
	- ie. `const int a = 3;`
- this makes the variable immutable - it can be only read, but not modified
- `const` arrays are a bit tricky, they cannot be overwritten in their entirety, but elements still can be changed
	- however, strings are fully immutable!

## reference and value types

- value types are types such as int, float or bool, they hold the data directly
	- stack memory
- reference types hold a reference to the actual data instead, such as arrays, dictionaries or strings
	- heap memory

## scope

- variables can be defined either globally, or in a scope
- a globally defined variable is accessible anywhere in the code
- a variable defined in a scope is accessible in the given scope
- a scope can be found in `if` statements, `for` or `while` loops and mainly function definitions
	- usually, indentation shows scopes pretty well
	- `var` is a funny little joker! we shall not speak of him :sob:

## typecasting

- converting one data type into another
- for example `int("3")` or `str(3)` in python
- in certain directions, such as number -> string, a success is guaranteed
- in other cases, such as string -> number, errors can occur
	- ie. `int("hello")`, hello is not a valid number
		- thats where `NaN` comes in from JS!
- there is also the possible loss of data (implicit x explicit casting)
	- `float` to `int` loses data because the decimal values get truncated
		- -> explicit
	- `int` to `float` does not lose data because there is no truncation needed
		- -> implicit