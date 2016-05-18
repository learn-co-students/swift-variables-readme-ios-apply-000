# Variables & Constants

## Learning Objectives

* Explain the following piece of code correctly. We declared a new variable called favoriteCharacter and gave it a value of Jon Snow.

```swift
var favoriteCharacter = "Jon Snow"
```

* Create a variable in a playground file.
* Change the value of a variable to another value (of the same type).
* Explain how a constant is used and why it differs from a variable. (let/var)
* Recognize the error produced when you attempt to change the value of a constant to something else.
* Explain why we have both options and how best we can make the choice between using a variable/constant.  

## What the Student Already Knows  
Nothing 🖖🏼 - this will be the first reading.

## Variables

_Variables_ are the fundamental building block of any program. A variable associates a _name_ with a _value_. That value can be almost anything: a number, a string (or sequence of characters), or even an object (which you will learn about in a future lesson). For instance, the following is a variable declaration in Swift:

```
var favoriteCharacter = "Jon Snow"
```

In the above example, a variable is declared using the `var` keyword. The name of the variable is `favoriteCharacter`. This variable has the value "Jon Snow". "Jon Snow" is a _string_, or sequence of characters enclosed in double quotation marks.

You can refer to this variable using its name. While the variable's value is initially "Jon Snow", it can change over time. For example, you could change it to "Tyrion Lannister":

```
favoriteCharacter = "Tyrion Lannister"
```

From here on out, `favoriteCharacter` will have the value "Tyrion Lannister", instead of "Jon Snow". Notice, however, that you didn't have to put `var` in front of `favoriteCharacter` when you changed the value. This is because you have already declared `favoriteCharacter` to be a variable, and so Swift knows that it exists. You're not _declaring_ a variable here; you're just changing its value to something else.

In Swift, every variable has a _type_. The type tells you the kind of value that variable refers to. In the above example, the type of the variable is a `String`. Other types include `Int` and `Double`. You will learn about many more of Swift's data types as you work through these lessons. For now, don't worry much about the type; just be aware that every variable has a type.

The type of a variable is important, because it can only hold values of the same type, even if you change the value. `favoriteCharacter` must always be a string—it cannot change to an `Int` or a `Double`.

Take a look at the [playground](Variables.playground) for this lesson. You can see how a variable in Swift is declared, and how you can change the value. Try it for yourself! Change `favoriteCharacter` to _your_ favorite character and see what happens.

## Constants

Swift offers a second way to associate a name with a value: a _constant_. Like a variable, a constant consists of a name and an associated value. Unlike a variable, however, the value of a constant cannot change over time; once you _initialize_ a constant (declare it and set it to a value), you cannot change it. Ever.

A Swift constant is declared like a variable, except it uses the keyword `let` instead of `var`:

```
let ultimateFavoriteCharacter = "Arya Stark"
```

From here on out, `ultimateFavoriteCharacter` will always have the value "Arya Stark". If you try to change it:

```
ultimateFavoriteCharacter = "Daenerys Targaryen"
```

You will get an error from the Swift compiler. Check out the [playground](Variables.playground) to see this for yourself. You will see an error issued on line 10.

Like variables, constants also have a type. Since you cannot change the value of a constant, you won't have to worry about changing the value to a different type. However, the type of constants still matters, since it dictates how you can interact with and use the constant, as you'll learn as you progress through your Swift studies.

## Using Variables and Constants

Why use variables and constants in your program? Both variables and constants are useful when you want to associate a name that never changes with a value that may change. You can then refer to that variable by a constant name. As shown in the playground associated with this lesson, once you associate the name `favoriteCharacter` with a value ("Jon Snow", for example), you can use `favoriteCharacter` to refer to that value for the rest of the program, such as when you pass it to functions like `print()`. (You will learn more about functions in a future lesson.)

## Choosing Between Variables and Constants

When should you use a variable, and when should you use a constant? A variable should be used when a value might change during the course of a single run of a program. For example, when you start running a program, your favorite may be Jon Snow, but perhaps by the end of the program's run, you may want to switch your allegiance to another character. A constant, on the other hand, is a way to bind a name to a value that won't change. This lets you refer to that value using a label without being concerned with the exact value that label takes.

<a href='https://learn.co/lessons/Variables' data-visibility='hidden'>View this lesson on Learn.co</a>
