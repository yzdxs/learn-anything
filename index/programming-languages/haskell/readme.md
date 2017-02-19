#[programming languages - haskell](https://my.mindnode.com/tecLyqHsjQf416hxx1LzXnNY6Hhx6gpUx9qRtv42)

![](http://i.imgur.com/35pcKxU.png)

#mindmap index 🗄️

# functor


## notes

### [a theoretical super-interface of Function, Iterable and friends, Optional, and many, many other parameterised types](http://jnape.com/the-perils-of-implementing-functor-in-java/)


# notes


## [haskell lessons](https://www.reddit.com/r/haskell/comments/5rcfyd/haskell_maxims_and_arrows/)

### Haskell is the promise that you can write it as cleanly as your understanding of it. Have faith.

### Always be looking for patterns. Abstract them always and only when it simplifies.

### Persevere in getting an abstraction just right. When you find it, everything will magically fall into place

### The implementation is the design.

### Hide whatever the caller shouldn't care about. In particular, you can remove type parameters with appropriate quantification.

### There's a reason fst3, snd3, thd3 are not in base. Triple or bigger: create a data type with fields instead.

### Never make an instance unless it morally follows the class's rules.

### Instances of simpler classes are more valuable than of more complex generalisations.

### Monoid: not a flashy class, but still definitely worthwhile.

### Applicative: hugely underappreciated, and good for types that have "static information". Lets you do deep magic with traverse and sequenceA.

### Monad: potential instances are usually easy to spot.

### The fewer type parameters in a class, the better. Can you turn any into associated types? Can you split the class into two classes? Can you hive off some of the parameters into a superclass?

### Don't worry about strictness until it's time to optimise.

### 1	Intuition about optimisation tends to be bad. Before profiling, limit yourself to reasoning about complexity classes.

### An orphan instance is a very minor wart.

- orphan instances might be a minor wart for application code, but they are a **major wart for libraries**.

- Do not put orphan instances in libraries when neither the class nor the type were defined by you. Two packages defining the same instance will cause massive headaches down the line—they'll cause conflicts for anybody who depends on both, even transitively.

### Types themselves are weightless (i.e., erased). For example, * dropped from kind to type (with TypeInType) carries no information.

### You probably won't need IORef

### Template Haskell comes with a high cost in intelligibility. Sometimes it's worth it.


# resources


## [haskell style guide](https://github.com/tibbe/haskell-style-guide)

## [official site](https://www.haskell.org/#step5)

## [write yourself a scheme in 48 hours](https://en.wikibooks.org/wiki/Write_Yourself_a_Scheme_in_48_Hours)

### RESEARCH: 



