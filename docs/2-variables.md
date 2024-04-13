# Variables

## Basic Variable Types
- `bool`
- `string`
- `int`
    - `rune` (alias for `int32`)
- `uint`
    - `byte` (alias for `uint8`)
- `float`
- `complex`

## Declaring Variables
- Variables are declared using the `var` keyword
- Value of an initialized variable with no assignment will be its [zero value](https://go.dev/tour/basics/12)

## Short Variable Declaration
- `:=` short assignment statement can be used in place of a `var` declaration
    - `:=` operator infers the type of the new variable based on the value
    
``` 
var empty string
```
is the same as

``` 
empty := ""
```

## Constants
- Value of a constant cannot change once declared
- Declared like variables but use the `const` keyword
- Constants must be known at compile time

## Formatting Strings
- `fmt.Printf` prints a formatted string to standard out
    - `%v`: Interpolate the default representation
    ```
    fmt.Printf("I am %v years old", 10)
    // I am 10 years old

    fmt.Printf("I am %v years old", "way too many")
    // I am way too many years old
    ```
    - `%s`: Interpolate a string
    - `%d`: Interpolate an integer in decimal form
    - `%f`: Interpolate a decimal

## Conditionals
- `if` statements in Go don't use parentheses around the condition
```
if height > 4 {
    fmt.Println("You are tall enough!")
}
```