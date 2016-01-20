これは OK!

```java
public void fuga() {
    Bar.invoke(5, new Foo() {
        @Override
        public int run() {
            return 15;
        }
    });
}
```

```java
public interface Foo
{
    int run();
}

public class Bar {
    public static void invoke(int count, Foo foo) {
        for (int i = 0; i < count; i++) {
            System.out.println(foo.run());
        }
    }
}
```
