# Adversarial dictionary learning for a robust analysis and modelling of spontaneous neuronal activity

This repository contains the official implementation of the proposed methods ADL and RADL described in the "Adversarial dictionary learning for a robust analysis and modelling of spontaneous neuronal activity".

[Paper Link](https://www.sciencedirect.com/science/article/pii/S0925231220300862?casa_token=_wAwet7U6oYAAAAA:TbeD-NqHBe5aCoSfIUzir7Ia3q-f57Gze3q3E5R1_ziHbf_K7CpmFshMhWKecCEBR9C3v5czDA)

# Abstract
The field of neuroscience is experiencing rapid growth in the complexity and quantity of the recorded neural activity allowing us unprecedented access to its dynamics in different brain areas. The objective of this work is to discover directly from the experimental data rich and comprehensible models for brain function that will be concurrently robust to noise. Considering this task from the perspective of dimensionality reduction, we develop an innovative, robust to noise dictionary learning framework based on adversarial training methods for the identification of patterns of synchronous firing activity as well as within a time lag. We employ real-world binary datasets describing the spontaneous neuronal activity of laboratory mice over time, and we aim to their efficient low-dimensional representation. The results on the classification accuracy for the discrimination between the clean and the adversarial-noisy activation patterns obtained by an SVM classifier highlight the efficacy of the proposed scheme compared to other methods, and the visualization of the dictionary’s distribution demonstrates the multifarious information that we obtain from it.

# Requirements

The code was tested on Matlab-R2019a

# Contents

**ADL/Adversarial_Dictionary_Learning:** The proposed method ADL that creates the dictionary.

**ADL/clean_noisy_examples_classification:** Function that trains and tests the classifier on clean and noisy data.

**ADL/column_merging:** Function that merges the columns of a matrix.

**ADL/OMP_non_normalized_atoms:** Function that decomposes sparse signals using the OMP algorithm.

**ADL/plot_dictionary_distribution:** Function that plots the distribution of the trained dictionary. 

**ADL/reconstructed_signals_testing:** Function that converts the real values of the reconstructed signal to 0 and 1.

**ADL/unwanted_columns_removal:** Function that removes zero columns and the columns having only one 1. 

-----

**RADL/Relaxed_Adversarial_Dictionary_Learning:** The proposed method RADL that creates the dictionary.

**RADL/clean_noisy_examples_classification:** Function that trains and tests the classifier on clean and noisy data.

**RADL/OMP_non_normalized_atoms:** Function that decomposes sparse signals using the OMP algorithm.

**RADL/plot_dictionary_distribution:** Function that plots the distribution of the trained dictionary. 

**RADL/reconstructed_signals_training_RADL:** Function that converts the real values of the reconstructed signal to 0 and 1.

**RADL/reconstructed_signals_testing_RADL:** Function that converts the real values of the reconstructed signal to 0 and 1.

**RADL/unwanted_columns_removal:** Function that removes zero columns and the columns having only one 1. 

**RADL/data_scaling:** Function that sums the values of the columns according to the size of the scale in an overlapping mode.

# Citation

Troullinou, E., Tsagkatakis, G., Palagina, G., Papadopouli, M., Smirnakis, S.M. and Tsakalides, P., 2020. Adversarial dictionary learning for a robust analysis and modelling of spontaneous neuronal activity. Neurocomputing, 388, pp.188-201.
