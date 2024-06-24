# AlgorithmicBias
Data Science in Action - Thesis on mitigating bias by applying various pre-processing techniques

# How to use this experiment?
First, download the files Measure.py and Generate_Samples.py. These should be in your main directory.
Then, download the files in the Py_Script.

It consists of three files: NoPreprocessing.ipynb, OverSampler/SMOTE and Fair-SMOTE.
Choose which treatment you would like to apply.

# Data Source, Ethics, Code, and Technology (DSECT) statement for this repository
The Data Source For this study, the data set has been acquired from the publicly available UC Irvine Machine Learning Depository and is part of the Statlog’s collection of datasets. The German Credit Dataset originated in 1994 and is provided by dr. Hans Hofmann, 1994 under the CC-BY 4.0 license. The data consists of anonymous data entries related to the credit risk based on various variables

Ethics: Figures: Most of the drawn figures are my own work. SHAP figures are generated from the shap packages. In the case that some figures are from a paper or other works, we make sure these papers are having an Creative Commons license (shown as CC-BY-NC-SA 4.0 following APA citation), or we have written permission from the au- thor. 

Code: The code is built in Python. A part of the code of calculating the fairness measures and the Fair-SMOTE algorithm has been derived from the author (Chakraborty et al., 2021), since these are not in packages. In that case, the reused code snippets will be properly mentioned as well as the license. It falls under the Apache 2.0 license, which means it may be redistributed, modified, as long as the original author is mentioned properly.

The full DSECT statement can be found in the thesis.

# Note about Measure.py and Generate_Samples.py
These files are the algorithms for measuring algorithmic bias and generating data points for Fair-SMOTE.
There are some small changes: adding a seed for reproducibility and generate column labels, and we removed the Mean Centering for the Disparate Impact metric.
These are derived from the GitHub repository of github.com/joymallac/Fair-SMOTE and from the papers of Chakraborty et al. (2021) Algorithmic Bias in Software? Why? How?.
The link to the paper is:[ https://arxiv.org/pdf/2105.12195](https://arxiv.org/abs/2105.12195)
It must be mentioned that the code for Measure.py and Generate_Samples.py are issued under the Apache 2.0 license by the author.

# Next iterations
There are some errors in the measurement of the Disparate Impact in the individual .ipynb files in the 'output' folder, since the metric's ideal value is 1.
In some papers, the DI is mean centered to 0 for interpretability.
The DI can be correctly measured with Measure.py's function. In the next commit, the mean centered version will be released.
