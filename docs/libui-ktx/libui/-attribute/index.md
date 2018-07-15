[libui-ktx](../../index.md) / [libui](../index.md) / [Attribute](./index.md)

# Attribute

`abstract class Attribute : `[`Disposable`](../-disposable/index.md)`<<ERROR CLASS>>`

Stores information about an attribute in a [string](../string.md).

### Constructors

| [&lt;init&gt;](-init-.md) | `Attribute(alloc: <ERROR CLASS><<ERROR CLASS>>?)`<br>Stores information about an attribute in a [string](../string.md). |

### Properties

| [type](type.md) | `val type: <ERROR CLASS>`<br>Returns the type of [Attribute](./index.md). |

### Inherited Properties

| [disposed](../-disposable/disposed.md) | `val disposed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Returns `true` if object was disposed - in this case [disposed](../-disposable/disposed.md) will do nothing, all other operations are invalid and will `throw Error("Resource is disposed")`. |
| [ptr](../-disposable/ptr.md) | `val ptr: <ERROR CLASS><`[`T`](../-disposable/index.md#T)`>` |

### Inherited Functions

| [dispose](../-disposable/dispose.md) | `open fun dispose(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Dispose and free all allocated native resources. |

### Inheritors

| [BackgroundAttribute](../-background-attribute/index.md) | `class BackgroundAttribute : `[`Attribute`](./index.md)<br>Changes the background color of the text it is applied to. |
| [ColorAttribute](../-color-attribute/index.md) | `class ColorAttribute : `[`Attribute`](./index.md)<br>Changes the color of the text it is applied to. |
| [FamilyAttribute](../-family-attribute/index.md) | `class FamilyAttribute : `[`Attribute`](./index.md)<br>Changes the font family of the text it is applied to. |
| [FeaturesAttribute](../-features-attribute/index.md) | `class FeaturesAttribute : `[`Attribute`](./index.md)<br>Creates a new Attribute that changes the font family of the text it is applied to. otf is copied you may free it after uiNewFeaturesAttribute() returns. |
| [ItalicAttribute](../-italic-attribute/index.md) | `class ItalicAttribute : `[`Attribute`](./index.md)<br>Changes the italic mode of the text it is applied to. |
| [SizeAttribute](../-size-attribute/index.md) | `class SizeAttribute : `[`Attribute`](./index.md)<br>Changes the size of the text it is applied to, in typographical points. |
| [StretchAttribute](../-stretch-attribute/index.md) | `class StretchAttribute : `[`Attribute`](./index.md)<br>Changes the stretch of the text it is applied to. |
| [UnderlineAttribute](../-underline-attribute/index.md) | `class UnderlineAttribute : `[`Attribute`](./index.md)<br>Changes the type of underline on the text it is applied to. |
| [UnderlineColorAttribute](../-underline-color-attribute/index.md) | `class UnderlineColorAttribute : `[`Attribute`](./index.md)<br>Changes the color of the underline on the text it is applied to. |
| [WeightAttribute](../-weight-attribute/index.md) | `class WeightAttribute : `[`Attribute`](./index.md)<br>Changes the weight of the text it is applied to. |
