<div align="center">
  
# Where, Why, and How is Bias Learned in Medical Image Analysis Models? A Study of Bias Encoding within Convolutional Networks using Synthetic Data

</div>

<p align="center">
<img src="figs/methods_fig.png?raw=true" width="600">
</p>

Code for layer-wise analysis of bias encoding in a CNN using SimBA data! Used in our paper: ["Where, Why, and How is Bias Learned in Medical Image Analysis Models? A Study of Bias Encoding within Convolutional Networks using Synthetic Data"]()

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
@article{,
	title={},
	DOI={},
	journal={},
	author={Stanley, Emma A M and Souza, Raissa and Wilms, Matthias and Forkert, Nils D},
	year={},
	pages={} }
```
```
Stanley, E.A.M., Souza, R., Wilms, M., Forkert, N.D. ....
```
