@title[Introduction]
## Why Learn Functiona Programming?

### Sharon Shmorak
---
@title[Transition]
# The meaning of Tingo
---?gist=abd45dfb2423ddd059c49cbbf8148207&lang=Java&title=Java GIST
@title[Simple data holding class in Java]
---?gist=06e83449bed463dc70687a686130906a&lang=Scala&title=Scala GIST
@title[Simple data holding class in Scala]
---
@title[Case class Sammery]
### Case class Sammery
* Concies
* Pragmatic equal sematics 
* Meanigful toString
* Support for Builder pattern
* Support for Pattern extraction
---
@title[Power and Responsibility]
### Greater Power Greater Responsibility
* More power to do things with functions
* More power to do things with types 
* Responsibility to keep functions pure
---
@title[More power to functions]
### More power to functions 
* pass as paramter and return as result
* pass by name 
### We gain laziness
```java
logger.debug(veryExpensiveCall())
```
```java
logger.debug(() -> veryExpensiveCall())
```
```
// Hoisted Function
public static final Function<String> veryExpensiveCallSupplier = 
  new Supplier<String>() {
    public String get() {
        return veryExpensiveCall();
    }
}; 

// Usage:
if (debugLevel == "debug")
  log(veryExpensiveCallSupplier.get())
```
---
@title[More power to types]
[Java-8-Lambdas-A-Peek-Under-the-Hood](https://www.infoq.com/articles/Java-8-Lambdas-A-Peek-Under-the-Hood)
### More power to work with types
### We can harness the compiler to help us in new ways
* Higher Kinded Type which looks like this ```Monad[T[_]]```
* [type classes and hd-hoc polymorphism](https://www.youtube.com/watch?v=1e9tcymPl7w)
* [type classes and build in dependency injection](https://www.youtube.com/watch?v=ZasXwtTRkio)
---
![lego_bricks](https://commons.wikimedia.org/wiki/File:2_duplo_lego_bricks.jpg)
### Where to learn more on Functional Programming in Java
[Functional Programming in Java](https://www.youtube.com/watch?v=TCJdc9SYwlQ)
[java8-stream-tutorial-examples](http://winterbe.com/posts/2014/07/31/java8-stream-tutorial-examples/)
---
### Where to learn more on Functional Programming in Scala
[scala-il on gitter](https://gitter.im/scala-il/Lobby)
[scala/scala on gitter](https://gitter.im/scala/scala)
[scale.bythebay.io: Rob Norris, Functional Programming with Effects](https://www.youtube.com/watch?v=po3wmq4S15A)

---
@title[because they are hard]
![Apollo_program](https://goo.gl/images/cn6bJm)
We choose to go to the Moon in this decade and do the other things,not because they are easy, but because they are hard; because that goal will serve to organize and measure the best of our energies and skills, because that challenge is one that we are willing to accept, one we are unwilling to postpone, and one we intend to win ...
