## Using ViewModifier
```swift
struct TitleModifier: ViewModifier {

    func body(content: Content) -> some View {
        content
            .font(.largeTitle)
    }

}
```

```swift
    var body: some View {
        Text("Bigger Text")
            .modifier(TitleModifier())
    }
```

## Using extension(much simpler💡）

```swift
extension View {

    func title() -> some View {
        self
            .font(.largeTitle)
    }

}
```

```swift
    var body: some View {
        Text("Bigger Text")
            .title()
    }
```
