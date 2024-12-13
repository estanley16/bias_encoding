<div align="center">
  
# Where, Why, and How is Bias Learned in Medical Image Analysis Models? A Study of Bias Encoding within Convolutional Networks using Synthetic Data

</div>

<p align="center">
<img src="figs/methods_fig.png?raw=true" width="600">
</p>

Code for layer-wise analysis of bias encoding in a CNN using SimBA data! Used in our [paper published in eBioMedicine.](https://www.thelancet.com/journals/ebiom/article/PIIS2352-3964(24)00537-1/fulltext)

* `layerwise_feature_extraction.ipynb`: extract image activations from an intermediate layer of a keras CNN
* `layerwise_encoding_analysis.ipynb`: analyze degree of linear separation (i.e., "encoding") of bias/disease information from the extracted activations

See [SimBA repo](https://github.com/estanley16/SimBA) for details on how to generate synthetic brain MRI with simulated biases and train counterfactual model pipelines. Will be updated soon with details on how to add multiple biases (e.g. intensity + morphology). :-) 


## Abstract
Background:
Understanding the mechanisms of algorithmic bias is highly challenging due to the complexity and uncertainty of how various unknown sources of bias impact deep learning models trained with medical images. This study aims to bridge this knowledge gap by studying where, why, and how biases from medical images are encoded in these models. 

Methods:
We systematically studied layer-wise bias encoding in a convolutional neural network for disease classification using synthetic brain magnetic resonance imaging data with known disease and bias effects. We quantified the degree to which disease-related information, as well as morphology-based and intensity-based biases were represented within the learned features of the model. 

Findings:
Although biases were encoded throughout the model, a stronger encoding didn’t always lead to the model using these biases as a shortcut for disease classification. We also observed that intensity-based effects had a greater influence on shortcut learning compared to morphology-based effects when multiple biases were present. 

Interpretation:
We believe that these results constitute an important first step towards a deeper understanding of algorithmic bias in deep learning models trained on medical imaging data. This study also showcases the benefits of utilizing controlled, synthetic bias scenarios for objectively studying the mechanisms of shortcut learning. 


## Citation
```
@article{stanley_ebiom_2025,
	title = {Where, why, and how is bias learned in medical image analysis models? A study of bias encoding within convolutional networks using synthetic data},
	volume = {111},
	doi = {10.1016/j.ebiom.2024.105501},
	journal = {eBioMedicine},
	author = {Stanley, Emma A. M. and Souza, Raissa and Wilms, Matthias and Forkert, Nils D.},
	month = jan,
	year = {2025},
	pages = {105501},
```
```
E. A. M. Stanley, R. Souza, M. Wilms, and N. D. Forkert, “Where, why, and how is bias learned in medical image analysis models? A study of bias encoding within convolutional networks using synthetic data,” eBioMedicine, vol. 111, p. 105501, Jan. 2025, doi: 10.1016/j.ebiom.2024.105501.
```
