@title[Introduction]
## Why Learn Functional Programming?

### Sharon Shmorak
---
@title[Transition]
# The meaning of Tingo
---?gist=06e83449bed463dc70687a686130906a&lang=Scala&title=Scala GIST
### More power...
* Concise
* Getters
* Reasonable equals semantics 
* Meanigful toString
* Support for Builder pattern
* Support for Powerful pattern matching mechanism 
@title[Simple data holding class in Scala]
@title[Simple data holding class in Java]
---?gist=abd45dfb2423ddd059c49cbbf8148207&lang=Java&title=Java GIST
---
@title[We gain laziness]
### For less work!
```java
// pass by value
logger.debug(veryExpensiveCall())
```
```java
// pass by name 
logger.debug(() -> veryExpensiveCall())
```
---
@title[The mind shift you can expect]
### To code as an artist or as an engineer? 
![lego_bricks](https://cdn.pixabay.com/photo/2013/10/04/18/09/lego-190704_960_720.jpg)
---
@title[firstWord]
```java
// “Hello world” -> “HelloHello”
duplicate(firstWord(message));
```
---
@title[FP style composition]
```java
Optional<String> firstWord(String message) {
  String[] words = message.split(' ');
  if (words.length > 0) {
    return Optional.of(words[0]);
  } else {
    return Optional.empty();
  }
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
* reuse code like Lego bricks
* Get one step closer to being engineer by 
* Many other resons but none that can fit in 10 min ignite talk
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
