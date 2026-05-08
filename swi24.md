# SWI 24

## programming languages

- all programming languages are built upon machine code
	- -> instructions for the cpu on what to do
- they allow the user to create various programs, websites, scripts and more
- each language has a different structure, depth (high level/low level) and focus

## compilation to machine code

- there are three types of languages in regards to compilation:
	1) compiled languages (C, C++, Rust, Nim, Zig, Haskell) - the whole program is compiled into machine code using a compiler before it is ever ran; the result is a binary file (.exe in Windows or .x86-64 in linux for example)
		- main advantage is performance - no need for compilation whilst running the program
		- main disadvantage is the lack of flexibility and compatibility - all data structures, etc. need to be defined before compilation and the binary is system-specific
	2) interpreted languages (Python, JavaScript, Lua, TypeScript) - there is no compilation or creation of a binary, code is translated on the go (JIT compilers)
		- main advantage is flexibility - arrays do not need to be defined, variables dont have to have a set type (with the exception of TypeScript); since the code is compiled during runtime, it is also not platform specific
		- main disadvantage is performance - JS is not that bad, but languages like Python are overall slower than compiled languages, since everything needs to be compiled and then executed when using the program
	3) inbetweeners (Java, C#) - both languages create intermediate code, where it is indeed compiled, but not fully to machine code (CIL in C#, .jar files in Java); the file is then executed in a virtual machine on the given device (JVM for Java, CLR for C#)
		- these languages usually have both the advantages from interpreted and compiled languages, however, the system itself is more complicated

## .NET

- an open-source and cross-platform framework and ecosystem from Microsoft
- uses the C#, F# or VB.NET language
- code gets compiled into CIL (common intermediate language), then gets run in the CLR (common language runtime), the .NET-specific virtual machine