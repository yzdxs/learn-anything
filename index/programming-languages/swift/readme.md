#[programming languages - swift](https://my.mindnode.com/ytMugWzTWi9FU2ysEdmKetyucqbdXrTzhUFyecdw)

![](http://i.imgur.com/7VUmhGe.png)

#mindmap index 🗄️

# learning


## [great video series](https://www.youtube.com/channel/UC4PxbUhXl1W9AjphmCx06vg/videos)

## [Building A Simple iOS Calculator App ](http://www.thomashanning.com/building-a-simple-ios-calculator-app-part-1/?utm_source=ReviveOldPost&utm_medium=social&utm_campaign=ReviveOldPost)

### TODO: 


# interesting projects


## [swisp - lisp in swift](https://github.com/jakerockland/Swisp)

## [TinyConsole](https://github.com/Cosmo/TinyConsole)

## [Trace](https://github.com/voidref/Trace)

### ray tracer in swift


# notes


## UILabel and UIButton are subclasses of UIView thus I can call them where UIView parameter is expected

## _ symbol eliminates the keyword when you call the method

### essentially it means that you do not have to name the parameter when calling the method

### obj.methodName(button)  
    
  // no need for  
  obj.methodName(sender: button)

## Optional containing nothing will crash your program at runtime ✨


# optionals


## The ? identifier means that the variable is optional, meaning its value can be nil.

### If you have a value in your code, declaring it as non-optional allows the compiler to check at build time if it has a chance to become nil.

### You can check whether it is nil in an if statement


# articles


## [Design Patterns in Swift](https://shirazian.wordpress.com/2016/04/11/design-patterns-in-swift/)

## [Building a LISP from scratch with Swift ✨](https://www.uraimo.com/2017/02/05/building-a-lisp-from-scratch-with-swift/)

### 


# optionals


## You cannot send a message to an Optional without unwrapping it.

### Optionals them‐ selves don’t respond to any messages. (Well, they do respond to some messages, but very few, and you are unlikely to use them — and in any case they are not the mes‐ sages to which the thing inside them responds.)

### If you try to send to an Optional a message intended for the thing inside it, you will get an error message from the com‐ piler:

## important use of Optionals is to defer initialisation of an instance property. If a variable (declared with var) is typed as an Optional, it has a value even if you don’t initialise it — namely nil.

### That comes in very handy in situations where you know something will have a value, but not right away. A typical example in real-life iOS programming is an outlet, which is a reference to something in your interface such as a button:


# collection types


## 


# resources


## [algorithms in swift ✨](https://github.com/raywenderlich/swift-algorithm-club)

### RESEARCH: go through fully

## [How To Build A SpriteKit Game In Swift 3](https://www.smashingmagazine.com/2016/11/how-to-build-a-spritekit-game-in-swift-3-part-1/)

### RESEARCH: 

## [hacking with swift](https://www.hackingwithswift.com/read)

### have to pay for it


# inheritance


# videos


## [What Haskell Taught Me About Writing Swift](https://realm.io/news/swift-summit-abizer-nasir-lessons-from-haskell/)

### 

### 

### 

### you can reason about your problem in terms of the types and transformations of those types, before writing any code

- 

### don’t have state, have functions that return values

- although this is easier said than done

### higher order functions can be used to reduce duplication in code

### aim to write small, pure functions with no side effects

### avoid mixing pure and impure code

### aim to write small, obviously correct functions

### 

### 

### 

### 

### OOP concerns data objects and operations on those data objects

### READ: 

