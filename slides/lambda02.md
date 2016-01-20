こんなふうに書ける!

```java
people.stream()
        .map(p -> "[" + p.name + "]")
        .forEach(name -> System.out.println(name));
```
