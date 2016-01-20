これが NG なのが致命的!

```java
public void fuga() {
    int i = 0;
    
    Bar.invoke(5, new Foo() {
        @Override
        public int run() {
            return i++;
        }
    });
}
```

あくまで個人の感想です... <!-- .element: class="fragment" data-fragment-index="1" -->
