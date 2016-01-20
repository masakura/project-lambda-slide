ラムダ式/クロージャーを使えばこんなにスッキリなのに! (C#)

```csharp
public void Fuga()
{
    int i = 0;

    Bar.Invoke(5, () => i++);
}
```
