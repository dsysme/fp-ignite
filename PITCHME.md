@title[Introduction]
## Why Learn Functional Programming?

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
### Case class Summery
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
---
@title[We gain laziness]
### We gain laziness
```java
logger.debug(veryExpensiveCall())
```
```java
logger.debug(() -> veryExpensiveCall())
```
```java
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
[Java-8-Lambdas-A-Peek-Under-the-Hood](https://www.infoq.com/articles/Java-8-Lambdas-A-Peek-Under-the-Hood)
---
@title[More power to types]
### More power to work with types
* Higher Kinded Type which looks like this ```Monad[T[_]]```
* type classes
---
### We can harness the compiler to help us in new ways
* Safer safe type langauge
* [hd-hoc polymorphism](https://www.youtube.com/watch?v=1e9tcymPl7w)
* [build in dependency injection](https://www.youtube.com/watch?v=ZasXwtTRkio)
---
@title[Computations as Lego bricks]
### Computations as Lego bricks
![lego_bricks](https://upload.wikimedia.org/wikipedia/commons/0/0f/2_duplo_lego_bricks.jpg)

---?gist=e0f55ca02c18f23ed759073c2b333a54&lang=Java&title=firstWord
@title[firstWord]
Origin: [Practical Functional Programming by @stevenheidel](https://hackernoon.com/practical-functional-programming-6d7932abc58b)

---?gist=70f24137de9e7b6f65b777df63b1e355&lang=Java&title=firstWord and duplicate
@title[Unsafe composition]
Origin: [Practical Functional Programming by @stevenheidel](https://hackernoon.com/practical-functional-programming-6d7932abc58b)

---?gist=eb0525f0a9525cdf949c687c78adb75f&lang=Java&title=firstWord and duplicate
@title[FP style composition]
Origin: [Practical Functional Programming by @stevenheidel](https://hackernoon.com/practical-functional-programming-6d7932abc58b)

---?gist=7a957907348432b947f86893d28918e0&lang=Scala
@title[For comprehension with Option]

---?gist=d1887e11cffb4f298b518f5292765a6c&lang=Scala
@title[For comprehension with Future]
---
@title[Why learn FP?]
### Why Learn functional Programming?
@title[fp in Java]
---
@title[How to learn FP?]
### How to learn Functional Programing?
<br>
Not Alone! 
<br>
Find me on [scala-il on gitter](https://gitter.im/scala-il/Lobby)
<br>
[Follow my Personal log: Learning Scala and Functional Programming on Medium](https://medium.com/@sharon.shmorak)
## Thank you for listening
---
### More Resources 
[scala/scala on gitter](https://gitter.im/scala/scala)
<br>
[practical-functional-programming](https://hackernoon.com/practical-functional-programming-6d7932abc58b) by [@stevenheidel](https://hackernoon.com/@stevenheidel)
<br>
[scale.bythebay.io: Rob Norris, Functional Programming with Effects](https://www.youtube.com/watch?v=po3wmq4S15A)
<br>
[For: What is it good for?—Josh Suereth & Dick Wall](https://www.youtube.com/watch?v=WDaw2yXAa50)
<br>
[Functional Programming in Java](https://www.youtube.com/watch?v=TCJdc9SYwlQ)
<br>
[java8-stream-tutorial-examples](http://winterbe.com/posts/2014/07/31/java8-stream-tutorial-examples/)
<br>
[The Neophyte's Guide to Scala](http://danielwestheide.com/scala/neophytes.html)
<br>
