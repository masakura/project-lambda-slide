がんばればいけるわけなんだけど...

```java
public void fuga() {
    int i = 0;
    
    Bar.invoke(5, new FooImpl(i));
}

class FooImpl implements Foo {
    private int _i;
    
    public FooImpl(int i) {
        _i = i;
    }
    
    @Override
    public int run() {
        return _i++;
    }
}
```
<!-- .element style="font-size: 50%" -->
