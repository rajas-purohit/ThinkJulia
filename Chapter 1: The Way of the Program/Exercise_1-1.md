# Exercise 1-1

Whenever you are experimenting with a new feature, you should try to make mistakes. For example, in the “Hello, World!” program, what happens if you leave out one of the quotation marks? What if you leave out both? What if you spell println wrong?

This kind of experiment helps you remember what you read; it also helps when you are programming, because you get to know what the error messages mean. It is better to make mistakes now and on purpose rather than later and accidentally.

1. In a print statement, what happens if you leave out one of the parentheses, or both?
```Julia
julia> println("hello friend!"

```

```Julia
julia> println"hello friend!"
ERROR: LoadError: UndefVarError: `@println_str` not defined in expression starting at REPL[14]:1
```

2. If you are trying to print a string, what happens if you leave out one of the quotation marks, or both?
```Julia
julia> println("hello friend!)

```

```Julia
julia> println(hello friend!)
ERROR: syntax: missing comma or ) in argument list
Stacktrace:
 [1] top-level scope
   @ none:1
```

3. You can use a minus sign to make a negative number like -2. What happens if you put a plus sign before a number? What about 2++2?

```Julia
julia> 2++2
ERROR: UndefVarError: `++` not defined
Stacktrace:
 [1] top-level scope
   @ none:1
```

```Julia
julia> +2
2
```

4. In math notation, leading zeros are okay, as in 02. What happens if you try this in Julia?
```Julia
julia> 02
2
```

5. What happens if you have two values with no operator between them?
```Julia
julia> 3 17
ERROR: syntax: extra token "17" after end of expression
Stacktrace:
 [1] top-level scope
   @ none:1
```
