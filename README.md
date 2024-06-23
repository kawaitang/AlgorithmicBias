# AlgorithmicBias
Data Science in Action - Thesis on mitigating bias by applying various pre-processing techniques



# Data Source, Ethics, Code, and Technology (DSECT) statement for this repository
The Data Source is from .

Ethics: All sources, whether it originates from ..., 

Code: Some code is derived from arVix publications of .

Technology: We make use of the following technical set-up:

# Note about Measure.py and Generate_Samples.py
These files are the algorithms for measuring algorithmic bias and generating data points for Fair-SMOTE.
There are some small changes: adding a seed for reproducibility and generate column labels, and we removed the Mean Centering for the Disparate Impact metric.
These are derived from the GitHub repository of github.com/joymallac/Fair-SMOTE and from the papers of Chakraborty et al. (2021) Algorithmic Bias in Software? Why? How?.
The link to the paper is:[ https://arxiv.org/pdf/2105.12195](https://arxiv.org/abs/2105.12195)
It must be mentioned that the code for Measure.py and Generate_Samples.py are issued under the Apache 2.0 license by the author.

# Next iterations
There are some errors in the measurement of the Disparate Impact in the .ipynb files, since the metric's ideal value is 1.
The DI can be correctly measured with Measure.py's function. In the next commit, the mean centered version will be released.
