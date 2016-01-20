これも OK!

```java
public void fuga(final int i) {
    //           ~~~~~ final つければ OK!
    Bar.invoke(5, new Foo() {
        @Override
        public int run() {
            // 定数化された引数を利用
            return i;
        }
    });
}
```
