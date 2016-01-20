C# では...

以下の場合は関数オブジェクトになります

```csharp
public void Fuga()
{
    Bar.Invoke(5, () => 0);
}
```

以下の場合は暗黙のクラスが作られます

```csharp
public void Fuga()
{
    var i = 0;

    Bar.Invoke(5, () => i++);
}
```

計測していないから分からないけど、Java はクロージャーをサポートしないから速いってことはなさそう。 <!-- .element: class="fragment" data-fragment-index="1" -->
