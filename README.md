# Variables & Constants

![Leo](http://i.imgur.com/GAoVBVG.jpg?1)

> Simplicity is the ultimate sophistication. —[Leonardo da Vinci](https://en.wikipedia.org/wiki/Leonardo_da_Vinci)

## Overview

In this lesson we'll define, create, and explain the differences between variables and constants. 

## Learning Objectives

* Create a variable in a playground file
* Change the value of a variable to another value of the same type
* Explain how a constant is used and why it differs from a variable
* Recognize the error produced when attempting to change the value of a constant
* Distinguish when to use a variable and when to use a constant

## Variables

_Variables_ are the fundamental building block of any program. A variable associates a _name_ with a _value_. That value can be almost anything: a number, a string (or sequence of characters), or even an object (which you will learn about in a future lesson). For instance, the following is a variable declaration in Swift:

```swift
var favoriteCharacter = "Jon Snow"
```

In the above example, a variable is declared using the `var` keyword. The name of the variable is `favoriteCharacter`. This variable has the value "Jon Snow". "Jon Snow" is a _string_, or sequence of characters enclosed in double quotation marks.

You can refer to this variable using its name. While the variable's value is initially "Jon Snow", it can change over time. For example, you could change it to "Tyrion Lannister":

```swift
favoriteCharacter = "Tyrion Lannister"
```

From here on out, `favoriteCharacter` will have the value "Tyrion Lannister", instead of "Jon Snow". Notice, however, that you didn't have to put `var` in front of `favoriteCharacter` when you changed the value. This is because you have already declared `favoriteCharacter` to be a variable, and so Swift knows that it exists. You're not _declaring_ a variable here; you're just changing its value to something else.

In Swift, every variable has a _type_. The type tells you the kind of value that variable refers to. In the above example, the type of the variable is a `String`. Other types include `Int` and `Double`. You will learn about many more of Swift's data types as you work through these lessons. For now, don't worry much about the type; just be aware that every variable has a type.

The type of a variable is important, because it can only hold values of the same type, even if you change the value. `favoriteCharacter` must always be a string—it cannot change to an `Int` or a `Double`. Remember when you changed `favoriteCharacter` to be "Tyrion Lannister" instead of "Jon Snow"? You were able to do that because `favoriteCharacter` is a `String` and both of those are `String`s. What happens if you tried to change `favoriteCharacter` to a number?

```swift
favoriteCharacter = 76
```

If you tried to do that, Swift would've spit out an error telling you that you cannot assign a variable of type `String` to an `Int`, and your program would not run.

Take a look at the [playground](https://github.com/learn-co-curriculum/swift-variables-readme/blob/master/Variables.playground/Contents.swift) for this lesson. You can see how a variable in Swift is declared, and how you can change the value. Try it for yourself! Change `favoriteCharacter` to _your_ favorite character and see what happens.

## Constants

Swift offers a second way to associate a name with a value: a _constant_. Like a variable, a constant consists of a name and an associated value. Unlike a variable, however, the value of a constant cannot change over time; once you _initialize_ a constant (declare it and set it to a value), you cannot change it. Ever.

A Swift constant is declared like a variable, except it uses the keyword `let` instead of `var`:

```swift
let ultimateFavoriteCharacter = "Arya Stark"
```

From here on out, `ultimateFavoriteCharacter` will always have the value "Arya Stark". If you try to change it:

```swift
ultimateFavoriteCharacter = "Daenerys Targaryen"
```

You will get an error from the Swift compiler. Check out the [playground](Variables.playground) to see this for yourself. You will see an error issued on line 12.

Like variables, constants also have a type. Since you cannot change the value of a constant, you won't have to worry about changing the value to a different type. However, the type of constants still matters, since it dictates how you can interact with and use the constant, as you'll learn as you progress through your Swift studies.

## Using Variables and Constants

Why use variables and constants in your program? Both variables and constants are useful when you want to associate a name that never changes with a value that may change. You can then refer to that variable by a constant name. As shown in the playground associated with this lesson, once you associate the name `favoriteCharacter` with a value ("Jon Snow", for example), you can use `favoriteCharacter` to refer to that value for the rest of the program, such as when you pass it to functions like `print()`. (You will learn more about functions in a future lesson.)

## Choosing Between Variables and Constants

When should you use a variable, and when should you use a constant? A variable should be used when a value might change during the course of a single run of a program. For example, when you start running a program, your favorite character may be Jon Snow, but perhaps by the end of the program's run, you may want to switch your allegiance to another character (like when you changed the value of `favoriteCharacter` to "Tyrion Lannister"). A constant, on the other hand, is a way to bind a name to a value that won't change. This lets you refer to that value throughout your program where you are certain without a doubt that the value will _never_ change.

<p class='util--hide'>View <a href='https://learn.co/lessons/swift-variables-readme'>Variables and Constants</a> on Learn.co and start learning to code for free.</p>
