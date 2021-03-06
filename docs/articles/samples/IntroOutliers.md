---
uid: BenchmarkDotNet.Samples.IntroOutliers
---

## Sample: IntroOutliers

### Source code

[!code-csharp[IntroOutliers.cs](../../../samples/BenchmarkDotNet.Samples/IntroOutliers.cs)]

### Output

```markdown
 Method |                 Job | OutlierMode |     Mean |       Error |      StdDev |
------- |-------------------- |------------ |---------:|------------:|------------:|
    Foo |  DontRemoveOutliers |        None | 150.5 ms | 239.1911 ms | 158.2101 ms |
    Foo | RemoveUpperOutliers |   OnlyUpper | 100.5 ms |   0.1931 ms |   0.1149 ms |

// * Hints *
Outliers
  IntroOutliers.Foo: DontRemoveOutliers  -> 1 outlier  was  detected
  IntroOutliers.Foo: RemoveUpperOutliers -> 1 outlier  was  removed
```

### See also

* @docs.statistics