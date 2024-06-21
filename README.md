Just a fork of [capacitor-mlkit](https://github.com/capawesome-team/capacitor-mlkit) repo to fix the problem with Samsung A23 scan.

It sets default resolution on imageAnalysis to 4000 x 4000 on starScan method.

```java
ImageAnalysis imageAnalysis = new ImageAnalysis.Builder().setTargetResolution(new Size(4000,4000)).setBackpressureStrategy(ImageAnalysis.STRATEGY_KEEP_ONLY_LATEST).build();
```
