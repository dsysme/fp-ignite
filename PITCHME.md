@title[Introduction]
## Why Learn Functiona Programming?

### Sharon Shmorak
---
@title[Transition]
# The meaning of Tingo
@title[Simple data holding class in Java]
---?gist=abd45dfb2423ddd059c49cbbf8148207&lang=Java&title=Java GIST
@title[Simple data holding class in Scala]
---?gist=06e83449bed463dc70687a686130906a&lang=Scala&title=Scala GIST
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
[Java-8-Lambdas-A-Peek-Under-the-Hood](https://www.infoq.com/articles/Java-8-Lambdas-A-Peek-Under-the-Hood)
