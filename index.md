<<<<<<< HEAD
<img src = "https://user-images.githubusercontent.com/16887042/38399942-3f8f86da-3902-11e8-935e-c2f4446c77b8.png" alt = "J4 Logo" width = 100 />
=======
![j4 icon](https://j4lang.github.io/images/j4icon.png "j4 logo")
>>>>>>> 829aef098c6bbb20b4e8f53d16d1806deb8b9940

## Introduction
J4 does away with verbose, unreadable code and replaces it with a readable, understandable coding language that standardizes meaningful, beautiful code. This is made possible with whitespace matching and utilizing syntax that emphasize the flow of information. Along with these leaps forward in code structure, J4 simplifies coding conventions by handling the minutia of memory management and reinventing the outdated and arbitrary rules present in other languages.

J4 pulls inspiration from Swift, ELM, Python, and Lua

## Features
* .j4 File Extension
* Whitespace Sensitive
* Easy Array Creation
<<<<<<< HEAD
* Powerful Object Creation
=======
* Powerful Object
>>>>>>> 829aef098c6bbb20b4e8f53d16d1806deb8b9940
* First Class Functions
* Higher Order Functions
* Static Typing
* Strong Typing

### Operators

* Additive: `+`, `-`
* Multiplicative: `*`, `/`, `%`
* Exponentiation: `^`
* Relational: `<`, `>`, `>=`, `<=`, `=`
* Boolean: `and`, `or`

### Data Types

* Number: `2`, `8.0`, `3.1415926`
* Boolean: `true`, `false`
* String: `“a”`, `“hello world”
* Function: `addOne(x)`
* Array: [`“Martinez”`, `"Goocher"`, `"Hardy"`, `"Watkins”`]
<<<<<<< HEAD
* Object: `Color magenta <- new Color(1.0,0.0,1.0)`, `Color halfGray <- new Color(0.5)`
=======
* Object: `{name:“Sally”, age:25, delete(), duplicate()}`
>>>>>>> 829aef098c6bbb20b4e8f53d16d1806deb8b9940
* Comments: `~ Single line comment`
            `(~ Multi line comment ~)`

## Example Programs
J4 on the left, Javascript on the right

__Variable Declarations__

```
<<<<<<< HEAD
String name <- "j4"                               let name = “j4”;
Number age <- 1                                   let age = 1;
Boolean hasArrows <- true                         let hasArrows = true;
=======
String name <- "j4"                               let name = “j4”
Number age <- 1                                   let age = 1
Boolean hasArrows <- true                         let hasArrows = true
>>>>>>> 829aef098c6bbb20b4e8f53d16d1806deb8b9940
```

__Arithmetic__

```
Number x <- ((4 + 3) * (10 - 1) ^ 2) / 4                 x = ((4 + 3) * Math.pow((10 - 1), 2)) / 4;
```

__If Statements__

```
if i=2                                           if (i===2){
    f(i)                                             f(i);
else if i>5                                      } else if (i>5){
    g(i)                                             g(i);
else                                             } else{
    h(i)                                             h(i);
                                                 }
```

__For Statements__

```
for Number i<-1, i<7, i<-i+1                      for (let i=1; i<7; i++) {
    f(i)                                              f(i);
                                                  }
```

__While Statements__

```
while i<7                                         while (i < 7) {
   f(i)                                               f(i);
                                                  }
```

__Functions__

```
Function twice(f:(Number) -> Number, x:Number) -> Number        var doTwice = (f, x) => {
    return f(f(x))                                                  return f(f(x));
                                                                }
Function addOne(x: Number) -> Number                            function addOne(x){
    return x+1                                                      return x+1;
                                                                }
```

__Concat__
To increase readibility and learnability, strings do not use the "+" operator
instead, the concat function is called to concatenate two or more strings
```
String s <- concat("Hello ", "World!")                  let s = "Hello" + "World";

```

__Object Declarations__

```
struct Color
<<<<<<< HEAD
  Number red, green, blue <- 0, 0, 0

  init(r: Number, g: Number, b: Number)
    self.red   <- r
    self.green <- g
    self.blue  <- b

  Function getColor(Nothing) -> Number[]
    Number[] rgb <- [self.red, self.green, self.blue]
    return rgb

Color magenta <- new Color(1.0,0.0,1.0)
=======
    Number red, green, blue
    init(red: Number, green: Number, blue: Number)
        self.red   <- red
        self.green <- green
        self.blue  <- blue

    init(grayscale: Number)
        red   <- grayscale
        green <- grayscale
        blue  <- grayscale

Color magenta <- new Color(1.0, 0.0, 1.0)
>>>>>>> 829aef098c6bbb20b4e8f53d16d1806deb8b9940
Color halfGray <- new Color(0.5)
```

### Semantic Analysis
* changedImmutableType : tried to change x from type Number to String.
* isNotAFunction : f is not a function
* isNotAnArray : l is not an array
* isNotAnObject : d is not an object
<<<<<<< HEAD
* doesNotHaveProperty : x does not have property x.property
=======
* doesNotHaveProperty : x does not have property x.size
>>>>>>> 829aef098c6bbb20b4e8f53d16d1806deb8b9940
* invalidBinaryOperands : List and Number cannot be used with +
* invalidUnaryOperand : String cannot be used with ‘not’
* parameterArgumentMismatch : f has signature Number, Array but was called with signature String, Array, Number
* expressionIsNotTypeBoolean : x + 3 is type Number but must be type Boolean
<<<<<<< HEAD
* notDeclared : tried to use x before it was declared
* notInitialized : x is not given a value
* notDeclared : x has not been declared
* alreadyDeclared : x has already been declared
* returnOutsideFunction : found a return statement outside of a function
* typeMismatch : expected String got Number
* typeDoesNotExist : X y expects object ‘X’ is a type for variable y
* noClassConstructor : did not find a constructor in class C
* invalidAccessType : arr["2"], Cannot access a list using a string, need a number
* arrayIndexOutOfBounds : tried to access an element outside of the bounds of the array
=======
* ~unusedVariable : variable x is declared but never used
* notDeclared : tried to use x before it was declared
* notInitialized : x is not given a value
* returnOutsideFunction : found a return statement outside of a function
* ~multipleReturnsInABlock : found more than one return statement in a block
* typeMismatch : expected String got Number
* typeDoesNotExist : X y expects object ‘X’ is a type for variable y
* noClassConstructor : did not find a constructor in class C
* arrayIndexOutOfBounds : tried to access an element outside of the bounds of the array

(~) means warning
>>>>>>> 829aef098c6bbb20b4e8f53d16d1806deb8b9940
