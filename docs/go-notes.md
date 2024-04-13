# Go Notes

## Why Go?
- Go code generally runs faster than interpreted languages and compiles faster than other compiled languages
    - Interpreted language examples: Python, Javascript
    - Compiled language examples: C, C++, Rust
- Interpreted languages convert human writted/readable code into binary code that computers can understand during each runtime. It requires the use of the source code language "interpreter" to interpret the commands of the code.
- Compiled languages compile/convert the human code into binary code upfront and then output a compiled program that is independent from the source code language and can run directly from the OS (`helloworld.exe` for example)
- Go enforces strong and static typing
    - Variables can only have a single type (`string`, `int`, etc.)
    - Errors can be caught at compile time and not risk having to discover errors during runtime
- Go programs are lightweight on memory
    - Each program includes a small amount of "extra" code that's included in the executable binary
    - This is called "Go Runtime" and a purpose of it is to cleanup unused memory at runtime

## Variables
- Basic variable types
    - `bool`
    - `string`
    - `int`
        - `rune` (alias for `int32`)
    - `uint`
        - `byte` (alias for `uint8`)
    - `float`
    - `complex`