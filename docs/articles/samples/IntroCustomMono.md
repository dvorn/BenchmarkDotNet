---
uid: BenchmarkDotNet.Samples.IntroCustomMono
---

## Sample: IntroCustomMono

BenchmarkDotNet allows you to compare different runtimes, including Mono.
If you apply `[MonoJob]` attribute to your class we use your default mono runtime.
If you want to compare different versions of Mono you need to provide use the custom paths.
You can do this today by using the overloaded ctor of MonoJob attribute or by specifying the runtime in a fluent way.

### Source code

[!code-csharp[IntroCustomMono.cs](../../../samples/BenchmarkDotNet.Samples/IntroCustomMono.cs)]

### See also

* @docs.customizing-runtime