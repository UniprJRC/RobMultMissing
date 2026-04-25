
# Robust Multivariate Analysis with Missing Observations
**Marco Riani**<sup>1</sup>*, **Anthony C. Atkinson**<sup>2</sup>, **Luca Greco**<sup>3</sup>* , and **Aldo Corbellini**<sup>1</sup>

<sup>1</sup> Department of Economics and Management and Interdepartmental Research Centre for Robust Statistics

<sup>2</sup> London School of Economics

<sup>3</sup> Università Telematica Giustino Fortunato

<!--
<table>
  <tr>
    <td><img src="brush2.jpg" width="1024" height="392"></td>
  </tr>
</table>
-->

# Abstract
We develop a general framework for multivariate analysis with missing
observations, with particular emphasis on the computation and use of
Mahalanobis distances. When some entries are missing, the usual
Mahalanobis distance can only be computed on the observed coordinates,
yielding _partial_ distances that are not directly comparable across
units with different missingness patterns. To overcome this difficulty,
we study a class of adjustments that rescale partial Mahalanobis
distances to a common reference scale.

The proposed methodology is based on the EM algorithm for estimating
multivariate normal location and scatter in the presence of missing
values. We show that this framework allows the computation of adjusted
distances without explicit imputation. Seven adjustment methods are
considered, including moment-based, determinant-based, and
distributional transformations, as well as a model-based correction
derived from the conditional expectation of the complete-data
Mahalanobis distance. This _principled_ adjustment is shown to be
optimal under a mean squared error criterion.

We further extend the methodology to a robust context through a trimmed
EM algorithm, thereby combining missing-data estimation with outlier
detection. A simulation study compares the proposed adjustments in terms
of their ability to reconstruct the complete-data Mahalanobis
distances. Across a wide range of settings, the principled EM correction
consistently provides the best performance, while chi-square, Beta, and
standardization mappings provide useful alternatives.

Finally, we introduce a new graphical diagnostic for assessing whether
data are Missing Completely at Random (MCAR), based on the comparison of
Mahalanobis distances computed from complete rows with those obtained
when all rows are used. This graphical procedure is formalized through a
Monte-Carlo test. The methods are illustrated on a dataset of cows with
missing measurements, where the analysis reveals both multivariate
outliers and clear evidence against MCAR.

The proposed framework provides a flexible and robust approach to
multivariate analysis with missing data, combining statistical
interpretability, computational efficiency, and practical diagnostic
tools.


---

In the table below you can find  the original source (MATLAB live script): .mlx file and the corresponding .ipynb file. 

**MATLAB live script files**

The .mlx file 
contain both the code and the output that the code produces.

:eyes: To view the .mlx files click  on the "File Exchange button"

▶️ To run the .mlx files in the free MATLAB on line click on "Run in MATLAB Online". The repo will be automatically cloned. 

The Jupiter notebook version of the files is also given in the last column of the table below. Similarly to the .mlx files the Jupiter notebook files also contain both the code and the output produced by the code.

**Jupiter notebook files**

To view the .ipynb files click on the corresponding link.

To run the .ipynb files inside the agnostic environment jupiter notebook follow the instructions in the file
[ipynbRunInstructions.md](https://github.com/UniprJRC/MonitoringBook/blob/main/ipynbRunInstructions.md). 

Note: in order to run the files below you need to have [FSDA toolbox](https://https://www.mathworks.com/matlabcentral/fileexchange/72999-fsda-flexible-statistics-data-analysis-toolbox) installed. 



<!--
<style>
table th:first-of-type {
    width: 25%;
}
table th:nth-of-type(2) {
    width: 25%;
}
table th:nth-of-type(3) {
    width: 25%;
}
table th:nth-of-type(4) {
    width: 25%;
}
</style>


| FileName | View :eyes:  | Run ▶️  | Jupiter notebook | m format
| -------- | ---- | --- | ---- | ----|
|`codeFig1.mlx`: Code to create a Scatter Plot Matrix (SPM) of the 'citiesItaly2024' dataset using the FSDA function spmplot. | [![File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://viewer.mathworks.com/renderer?viewer=live_code&url=https%3A%2F%2Fwww.mathworks.com%2Fmatlabcentral%2Fmlc-downloads%2Fdownloads%2F3b230413-cbf8-4fa0-9df1-2a0cd1a401a8%2F1768209945%2Ffiles%2FcodeFig1.mlx&embed=web)  | [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=UniprJRC/PCAinteractive&file=codeFig1.mlx) | [codeFig1.ipynb](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig1.ipynb) | [codeFig1.m](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig1.m)
|`codeFig2to8.mlx`: This code generates Figures from 2 to 8. | [![File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://viewer.mathworks.com/renderer?viewer=live_code&url=https%3A%2F%2Fwww.mathworks.com%2Fmatlabcentral%2Fmlc-downloads%2Fdownloads%2F3b230413-cbf8-4fa0-9df1-2a0cd1a401a8%2F1767858305%2Ffiles%2FcodeFig2to8.mlx&embed=web&embed=web) |  [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=UniprJRC/PCAinteractive&file=codeFig2to8.mlx) | [codeFig2to8.ipynb](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig2to8.ipynb) | [codeFig2to8.m](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig2to8.m) |
|`codeFig9to15.mlx`: This code generates Figures from 9 to 15. | [![File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://viewer.mathworks.com/renderer?viewer=live_code&url=https%3A%2F%2Fwww.mathworks.com%2Fmatlabcentral%2Fmlc-downloads%2Fdownloads%2F3b230413-cbf8-4fa0-9df1-2a0cd1a401a8%2F1767858305%2Ffiles%2FcodeFig9to15.mlx&embed=web&embed=web) |   [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=UniprJRC/PCAinteractive&file=codeFig9to15.mlx) | [codeFig9to15.ipynb](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig9to15.ipynb) | [codeFig9to15.m](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig9to15.m)  |
|`codeFig16.mlx`: This code creates Figure from 16.   | [![File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://viewer.mathworks.com/renderer?viewer=live_code&url=https%3A%2F%2Fwww.mathworks.com%2Fmatlabcentral%2Fmlc-downloads%2Fdownloads%2F3b230413-cbf8-4fa0-9df1-2a0cd1a401a8%2F1767858305%2Ffiles%2FcodeFig16.mlx&embed=web&embed=web) |   [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=UniprJRC/PCAinteractive&file=codeFig16.mlx) | [codeFig16.ipynb](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig16.ipynb) | [codeFig16.m](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig16.m)    |
|`codeFig17to18.mlx`: This code generates Figures from 17 to 18.   | [![File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://viewer.mathworks.com/renderer?viewer=live_code&url=https%3A%2F%2Fwww.mathworks.com%2Fmatlabcentral%2Fmlc-downloads%2Fdownloads%2F3b230413-cbf8-4fa0-9df1-2a0cd1a401a8%2F1767858305%2Ffiles%2FcodeFig17to18.mlx&embed=web&embed=web) |   [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=UniprJRC/PCAinteractive&file=codeFig17to18.mlx) | [codeFig17to18.ipynb](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig17to18.ipynb) | [codeFig17to18.m](https://github.com/UniprJRC/PCAinteractive/blob/main/codeFig17to18.m)   |


---
-->

| Description | Routine name (link to HTML doc file)|
|---|---|
| EM algorithm for data with missing values (no trimming). | [`mdEM`](http://rosa.unipr.it/FSDA/mdEM.html) |
| EM algorithm with trimming (TEM) for data with missing values. | [`mdTEM`](http://rosa.unipr.it/FSDA/mdTEM.html) |
| Compute squared Mahalanobis distances using only observed entries. | [`mdPartialMD`](http://rosa.unipr.it/FSDA/mdPartialMD.html) |
| Rescale partial squared Mahalanobis distances to the full-dimensional scale. | [`mdPartialMD2full`](http://rosa.unipr.it/FSDA/mdPartialMD2full.html) |
| Bootstrap test for change in Mahalanobis distances under MCAR. | [`mdMCARtest`](http://rosa.unipr.it/FSDA/mdMCARtest.html) |
| Replace NaNs with conditional mean or random draw from conditional distribution. | [`mdImputeCondMean`](http://rosa.unipr.it/FSDA/mdImputeCondMean.html) |

![GitHub top language](https://img.shields.io/github/languages/top/UniprJRC/boot-TCLUST)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/UniprJRC/boot-TCLUST)
[![View on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/183001-pcainteractive)


[![GitHub contributors](https://img.shields.io/github/contributors/UniprJRC/boot-TCLUST)](https://github.com/UniprJRC/2025tobit/graphs/contributors)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/UniprJRC/boot-TCLUST/graphs/commit-activity)
![master](https://img.shields.io/github/last-commit/badges/shields/master)



