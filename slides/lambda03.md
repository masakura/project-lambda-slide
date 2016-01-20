並列化もお手のもの!

```java
people.parallelStream()
        .map(p -> "[" + p.name + "]")
        .forEach(name -> System.out.println(name));
```
