
## Facade Pattern 

***

```go
package facade

type Buffer struct {
        width, height int
        buffer        []rune
}

func (b *Buffer) At(index int) rune {
        return b.buffer[index]
}

func NewBuffer(width, height int) *Buffer {
        return &Buffer{width, height,
                make([]rune, width*height)}
}

type Viewport struct {
        buffer *Buffer
        offset int
}

func (v *Viewport) GetCharacterAt(index int) rune {
        return v.buffer.At(v.offset + index)
}

func NewViewport(buffer *Buffer) *Viewport {
        return &Viewport{buffer: buffer}
}


// a facade over buffers and viewports
type Console struct {
        buffers   []*Buffer
        viewports []*Viewport
        offset    int
}

func (c *Console) GetCharacterAt(index int) rune {
        return c.viewports[0].GetCharacterAt(index)
}

func NewConsole() *Console {
        b := NewBuffer(10, 10)
        v := NewViewport(b)
        return &Console{[]*Buffer{b}, []*Viewport{v}, 0}
}

func main() {
        c := NewConsole()
        u := c.GetCharacterAt(1)
}
```

***

![facade Pattern](images/facade.png)


***

[Facade in Go](https://refactoring.guru/design-patterns/facade/go/example)

Facade is a structural design pattern that provides a simplified (but limited) interface to a complex system of classes, library or framework.

![Conceptual Example](images/facade_golang.png)

