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