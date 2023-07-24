# Molang

A dynamically interpreted language that enables rapid development and efficiency

## Features of Molang

1. C-like syntax
2. variable bindings
3. comments
4. integers and booleans
5. arithmetic expressions
6. built-in functions
7. first-class and higher-order functions
8. closures
9. data structures such as string, array, and hash.

## Requirements
1. Go >= 1.20.3 

## Examples of Molang constructs
1. **Let statements**: They are used for assigning variables. All let statements always end with a semicolon as it is mandatory in Molang
   
   ```mg
      let a = 3 + 3;
   ```
3. **Functions**: In Molang, Functions are represented by `fn` and are regarded as first-class citizens, meaning you could do something like this:
   
   ```mg
     # Higher-order functions can be assigned to a variable and then called using that variable
     let add = fn(x, y) {
                  return x + y;
               };

     # calling the add function
     add(3, 3);

     # Function declarations
     fn add(x, y) {
        return x + y;
     };

     # Both functions above are essentially equivalent
   ```

## Roadmap to additional constructs to be added to Molang

These features were inspired by Typescript and Zig. These include

- [ ] add type hinting system - Late October
- [ ] add struct and enum data structure - Late October
- [ ] add support for generics - Mid-December
- [ ] add support for pattern-matching (Zig-style) - Next January or earlier

## Main goals of Molang

I started Molang to strengthen my knowledge of Golang and learn about concepts in the design of programming languages such as lexical analysis, parsing, syntax trees, the internal object system, evaluator, garbage collection, bytecode compilation, and so on.

## How to use
As Molang is still in early development, I have not come up with a build system or an installation guide. As such there is one way to test Molang and that is through the `REPL`. It can be accessed by running the command in the base directory of the Molang project: `go run main.go`
