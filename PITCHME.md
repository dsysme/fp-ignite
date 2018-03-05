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
* Concise
* Reasonable equals semantics 
* Meanigful toString
* Support for Builder pattern
* Extractor object to 
---
@title[Power and Responsibility]
### Greater Power Greater Responsibility
* More power to do things with functions
* More power to do things with types 
* Responsibility to keep functions pure
---
@title[More power to functions]
### More power to functions - Examples
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
### More power to work with types - Examples
* apply tools from Category theory
* [build in dependency injection](https://www.youtube.com/watch?v=ZasXwtTRkio)
* [hd-hoc polymorphism](https://www.youtube.com/watch?v=1e9tcymPl7w)
* Safer safe type langauge
---
@title[Computations as Lego bricks]
### Purity makes computations compose like Lego bricks
![lego_bricks](https://upload.wikimedia.org/wikipedia/commons/0/0f/2_duplo_lego_bricks.jpg)

---
@title[firstWord]
<script src="https://gist.github.com/stevenheidel/a374c47b11af279ff6be89faed37ff50.js"></script>
<script src="https://gist.github.com/stevenheidel/70f24137de9e7b6f65b777df63b1e355.js"></script>
<script src="https://gist.github.com/stevenheidel/eb0525f0a9525cdf949c687c78adb75f.js"></script>
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
* To gear you mind into becoming a better programmer
* To reuse your code like Lego bricks
* To fully exploit the power of the compiler to guard us from mistakes
* So you can be lazy: do more, do it more efficiently and with far less code 
* So you can have fun!
@title[fp in Java]
---
@title[How to learn FP?]
### How to learn Functional Programming?
<br>
Not Alone! 
<br>
<br>
Find me on [scala-il on gitter](https://gitter.im/scala-il/Lobby)
<br>
<br>
[Follow my Personal log: Learning Scala and Functional Programming on Medium](https://medium.com/@sharon.shmorak)
### Thank you for listening !!!
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
