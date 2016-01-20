クロージャーはだめでした...

```java
public void fuga() {
    int i = 0;
    
    Bar.invoke(5, () -> i++);
}
```

final 扱いにできる状態じゃないとだめっぽいです... <!-- .element: class="fragment" data-fragment-index="1" -->
