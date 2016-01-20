これは NG!

```java
public void fuga() {
    int i = 15;
    
    Bar.invoke(5, new Foo() {
        @Override
        public int run() {
            // スコープ外の変数は使えない
            return i;
        }
    });
}
```
