# Normalized Entropy

### Normalized Entropy [](#h2__1831139854){#h2__1831139854}

Normalized Entropy is a metric that takes into account the maximum possible value of Entropy and returns a normalized measure of the uncertainty associated with the variable:

$${H\_N}(X) = \frac{{ H(X) }}{{ {{\log }_2}({S_X}) }}$$

### Example [](#h2_1491730608){#h2_1491730608}

In this new example, we now compare the variables X1 and X2, which each represent ball colors:

- X1 ∈ {blue, red}
- X2 ∈ {blue, red, green, yellow, purple, orange, brown, black}

Normalized Entropy allows us to compare the degree of uncertainty even though these two variables have different numbers of states, i.e., two versus eight states:

|                                                          X1                                                          |                                                          X2                                                          |
| :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
|           ![](https://bayesia.clickhelp.co/resources/Storage/bayesialab/Information-Theory/Entropy/X1.svg)           |           ![](https://bayesia.clickhelp.co/resources/Storage/bayesialab/Information-Theory/Entropy/X2.svg)           |
| ![](https://bayesia.clickhelp.co/resources/Storage/bayesialab/Information-Theory/Entropy/BlueBalls25pct_300x169.png) | ![](https://bayesia.clickhelp.co/resources/Storage/bayesialab/Information-Theory/Entropy/AllColorsBalls_300x169.png) |

### Usage [](#h2_519852009){#h2_519852009}

In BayesiaLab, the values of Entropy and Normalized Entropy can be accessed in a number of ways:

- In Validation Mode ![](https://res.cloudinary.com/dvr3obmlj/image/upload/v1686184062/BayesiaLab_Icons/validation_ivi5eq.svg), with the Information Mode ![](https://res.cloudinary.com/dvr3obmlj/image/upload/v1686184081/BayesiaLab_Icons/tooltip_tndtk6.svg) activated, hovering over a Monitor with your cursor will bring up a Tooltip that includes Entropy and Normalized Entropy.

{% embed url="<https://res.cloudinary.com/dvr3obmlj/video/upload/v1690488783/MonitorEntropy_ifw8m2.mp4>" %}

- You can also sort the Monitors in the Monitor Panel according to their Normalized Entropy via `Monitor Context Menu > Sort > Normalized Entropy`.

![](https://bayesia.clickhelp.co/resources/Storage/bayesialab/Information-Theory/Entropy/Normalized-Entropy/MonitorContextMenuSortByNormalizedEntropy.png)

- The Normalized Entropy is also available as a Node Analysis metric for Size and Color in the 2D and 3D Mapping Tools.
- In Function Nodes, Entropy and Normalized Entropy are available as Inference Functions in the Equation tab.
  * Entropy: `Entropy(?X1?, False)`
  * Normalized Entropy: `Entropy(?X1?, True)`

### Demo Network [](#h2_1318485153){#h2_1318485153}

![](https://res.cloudinary.com/dvr3obmlj/image/upload/v1692036394/xbl3_xmnk2g.svg) [NormalizedEntropy.xbl](https://res.cloudinary.com/dvr3obmlj/raw/upload/v1690480310/NormalizedEntropy_jtqymx.xbl)
