# Evaluating saliency methods on artificial data with different background types

This repository contains the relevant code for the MedNeurips 2021 submission 'Evaluating saliency methods on artificial data with different background type', by Céline Budding, Fabian Eitel, Kerstin Ritter, and Stefan Haufe. The work was conducted when Céline Budding was a MSc student at the BCCN Berlin. In this work, we aimed to evaluated so-called saliency methods on artificial data with either a perlin noise or 2D brain MRI background. This showed that saliency methods are strongly affected by different background and lesions, and should be investigated and evaluated in more detail. 

Note that the code contained in this repository is preliminary: some more experiments have been conducted beyond the results reported in this manuscript, so the code may not be fully representative of the results. For example, the option to blur the Perlin and MRI samples has been added, and further experiments have also included alternative noise backgrounds. 

# How to use the code

The notebooks in this repository can be used to 1) generate the data (provided that a dataset with structural MRI images is available, nothing is required for the perlin data), 2) train a network and run saliency methods, 3) analyze the data qualitatively and quantitatively. 

- Generating the data: use the notebooks ```create_mri_data_lesions.ipynb``` and ```create_perlin_dataset.ipynb```. 
- Training the network: ```network_and_training.ipynb``` and ```saliency_methods.ipynb```. 
- Running the evaluation: ```overview_plots_qualitative.ipynb``` and ```result_plots_metrics.ipynb```. \

Note that the file paths should be changed to the respective file paths on one's system, and that the dimensions of the data and the GPU path might also need to be adapted.

This code is published under a BSD License 2.0. 
