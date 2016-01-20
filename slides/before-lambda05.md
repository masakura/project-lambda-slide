これは OK!

```java
public void fuga() {
    final int i = 15;
    // ~~ final つければ OK
    
    Bar.invoke(5, new Foo() {
        @Override
        public int run() {
            // スコープ外の定数を利用
            return i;
        }
    });
}
```
