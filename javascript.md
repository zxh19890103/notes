在 JavaScript 中, Number 是一种 定义为 [64位双精度浮点型](http://en.wikipedia.org/wiki/Double_precision_floating-point_format)（double-precision 64-bit floating point format） (IEEE 754)的数字数据类型。在其他编程语言中，有不同的数字类型存在，比如：整型（Integers），单精度浮点型（Floats），双精度浮点型（Doubles），大数（Bignums）。

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/IEEE_754_Double_Floating_Point_Format.svg/618px-IEEE_754_Double_Floating_Point_Format.svg.png)

e = 00000000001<sub>2</sub> = 001<sub>16</sub> = 1; 2<sup>1-1023</sup> = 2<sup>-1022</sup> *(smallest exp)*

e = 01111111111<sub>2</sub> = 3ff<sub>16</sub> = 1023; 2<sup>1023-1023</sup> = 2<sup>0</sup>  *(zero offset)*

e = 10000000101<sub>2</sub> = 405<sub>16</sub> = 1029; 2<sup>1029-1023</sup> = 2<sup>6</sup>

e = 11111111110<sub>2</sub> = 7fe<sub>16</sub> = 2046; 2<sup>2046-1023</sup> = 2<sup>1023</sup> *(highest exp)*

### special cases.

00000000000<sub>2</sub> = 000<sub>16</sub> = 0; represents a signed **ZERO**.

11111111111<sub>2</sub> = 7ff<sub>16</sub> = 2047; represents **infinite** (*if* F = 0) and NaNs (*if* F ≠ 0).

