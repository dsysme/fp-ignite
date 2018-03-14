@title[Introduction]
## Why Learn Functional Programming?

### Sharon Shmorak
---
@title[C++ to Java to Scala]
# C++ => JAVA != JAVA => FP/Scala
---
@title[Transition]
# The meaning of Tingo
---
@title[Case class]
### The meaning of case
```scala
case class Book(name: String, author: String)
```
* Getters
* Reasonable equals semantics 
* Meanigful toString
* Support for Builder pattern
* Support for Powerful pattern matching mechanism 
@title[Simple data holding class in Scala]
---?gist=abd45dfb2423ddd059c49cbbf8148207&lang=Java&title=Java GIST&file=Book.java
---
@title[The mind shift you can expect]
### Yes we can!
### אנחנו יכולים/יכולות
---
@title[We gain laziness]
### Why work hard when you can be lazy?
```java
// pass by value
logger.debug(veryExpensiveCall())
```
```java
// pass by name 
logger.debug(() -> veryExpensiveCall())
```
---
### To code as an artist or as an engineer? 
![Lego_bricks](https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/Lego_bricks.jpg/640px-Lego_bricks.jpg)
---
@title[firstWord]
```java
// “Hello world” -> “HelloHello”
duplicate(firstWord(message));
```
@title[FP style composition]
```java
Optional<String> firstWord(String message) {
  ...
}
```
```java
firstWord(input).map(this::duplicate)
```

Origin: [Practical Functional Programming by @stevenheidel](https://hackernoon.com/practical-functional-programming-6d7932abc58b)

---
@title[Why learn FP?]
### Why Learn functional Programming?
* To gear you mind into becoming a better programmer
* The artist in you should compose music not code! 
* You should compose code like Lego bricks
* Many other reasons but none that can be explained in less than 10 min
@title[fp in Java]
---
@title[How to learn FP?]
### How to learn Functional Programming?
<br>
Not Alone! 
<br>
<br>
Find good people at [Scala](https://gitter.im/scala/scala) and [scala-il](https://gitter.im/scala-il/Lobby) rooms on gitter
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
