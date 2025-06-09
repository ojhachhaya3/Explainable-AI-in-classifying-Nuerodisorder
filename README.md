# Explainable-AI-in-classifying-Nuerodisorder
## Overview

Explainable AI (XAI) refers to a set of techniques and methods that make the behavior of machine learning models understandable to humans. In healthcare and neuroscience, where high-stakes decisions are involved, interpretability is essential — not just for accuracy, but also for clinical trust, regulatory acceptance, and knowledge discovery.
The primary objective is to develop an interpretable machine learning pipeline that:
Classifies EEG recordings into Healthy and Schizophrenic classes.
Uses statistical features extracted from EEG signals.
Applies XAI techniques (e.g., SHAP, PDP, ICE) to understand why the model makes its decisions — enabling trust, transparency, and clinical insight and visualize how features influence model predictions.

for a detailed explaination, please check the [report](report.pdf)

## Dataset
Dataset is available in the paper[Graph-based analysis of brain connectivity in schizophrenia]and dataset contains electroencephalography (EEG) data from 14 patients with schizophrenia and 14 healthy controls.You can access the EEG data files from :
(https://drive.google.com/drive/folders/16j8TwPh92DjikvzWOfhN37qARd6vTdPc?usp=drive_link)

## Conclusion
SHAP and Integrated Gradients analyses highlight that argmax, argmin, kurtosis, and skewness are the most influential features, with argmax and argmin showing the highest impact on predictions, particularly at specific time steps (5–10 and 15–17.5).Partial Dependence Plots further confirm that higher skewness and kurtosis values increase the likelihood of schizophrenia prediction, while argmax and argmin exhibit non-linear effects. Feature importance rankings consistently place abs_diff_signal, maxim, and ptp as top contributors to model output magnitude.Collectively, these findings suggest that the model effectively captures temporal and statistical patterns in EEG data, particularly thetiming and shape of signal distributions, to differentiate schizophrenia patients from healthy controls, providing a robust foundation for clinical decision support. 

## Future Work
Expanding Data Volume, Investigate advanced data augmentation techniques specific to EEG signals to increase the dataset size artificially, improving the model's generalization ability without the need for additional data collection.
