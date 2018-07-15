[libui-ktx](../../index.md) / [libui](../index.md) / [Path](./index.md)

# Path

`class Path : `[`Disposable`](../-disposable/index.md)`<<ERROR CLASS>>`

Represent a path that could be drawed on a [DrawContext](../-draw-context.md)

### Constructors

| [&lt;init&gt;](-init-.md) | `Path(mode: <ERROR CLASS>)`<br>Represent a path that could be drawed on a [DrawContext](../-draw-context.md) |

### Inherited Properties

| [disposed](../-disposable/disposed.md) | `val disposed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Returns `true` if object was disposed - in this case [disposed](../-disposable/disposed.md) will do nothing, all other operations are invalid and will `throw Error("Resource is disposed")`. |
| [ptr](../-disposable/ptr.md) | `val ptr: <ERROR CLASS><`[`T`](../-disposable/index.md#T)`>` |

### Inherited Functions

| [dispose](../-disposable/dispose.md) | `open fun dispose(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Dispose and free all allocated native resources. |

### Extension Functions

| [arcTo](../arc-to.md) | `fun `[`Path`](./index.md)`.arcTo(xCenter: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, yCenter: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, radius: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, startAngle: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, sweep: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, negative: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = false): <ERROR CLASS>`<br>Adds an arc to the path which is centered at ([xCenter](../arc-to.md#libui$arcTo(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/xCenter), [yCenter](../arc-to.md#libui$arcTo(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/yCenter)) position with radius [radius](../arc-to.md#libui$arcTo(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/radius) starting at [startAngle](../arc-to.md#libui$arcTo(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/startAngle) and with sweep angle [sweep](../arc-to.md#libui$arcTo(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/sweep) going in the given direction by anticlockwise (defaulting to clockwise) as specified by [negative](../arc-to.md#libui$arcTo(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/negative). |
| [bezierTo](../bezier-to.md) | `fun `[`Path`](./index.md)`.bezierTo(c1x: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, c1y: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, c2x: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, c2y: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, endX: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, endY: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`): <ERROR CLASS>`<br>Adds a cubic Bézier curve to the path. It requires three points. The first two points are control points and the third one is the end point. The starting point is the last point in the current path. |
| [closeFigure](../close-figure.md) | `fun `[`Path`](./index.md)`.closeFigure(): <ERROR CLASS>`<br>Causes the point of the pen to move back to the start of the current sub-path. It tries to draw a straight line from the current point to the start. If the shape has already been closed or has only one point, this function does nothing. It end the path. |
| [figure](../figure.md) | `fun `[`Path`](./index.md)`.figure(x: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, y: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`): <ERROR CLASS>`<br>Starts a new figure at the specified point. Call this method when you want to create a new path. |
| [figureWithArc](../figure-with-arc.md) | `fun `[`Path`](./index.md)`.figureWithArc(xCenter: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, yCenter: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, radius: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, startAngle: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, sweep: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, negative: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = false): <ERROR CLASS>`<br>Starts a new figure and adds an arc to the path which is centered at ([xCenter](../figure-with-arc.md#libui$figureWithArc(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/xCenter), [yCenter](../figure-with-arc.md#libui$figureWithArc(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/yCenter)) position with radius [radius](../figure-with-arc.md#libui$figureWithArc(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/radius) starting at [startAngle](../figure-with-arc.md#libui$figureWithArc(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/startAngle) and with sweep angle [sweep](../figure-with-arc.md#libui$figureWithArc(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/sweep) going in the given direction by anticlockwise (defaulting to clockwise) as specified by [negative](../figure-with-arc.md#libui$figureWithArc(libui.Path, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Double, kotlin.Boolean)/negative). |
| [lineTo](../line-to.md) | `fun `[`Path`](./index.md)`.lineTo(x: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, y: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`): <ERROR CLASS>`<br>Connects the last point in the subpath to the x, y coordinates with a straight line. |
| [rectangle](../rectangle.md) | `fun `[`Path`](./index.md)`.rectangle(x: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, y: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, width: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`, height: `[`Double`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-double/index.html)`): <ERROR CLASS>`<br>Creates a path for a rectangle at position (x, y) with a size that is determined by width and height. |
