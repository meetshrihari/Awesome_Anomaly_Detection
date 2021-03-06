<div style="border-bottom:none;">
  <div align="center">
    <img src="Img/algo.png" width="300">
    <h1>Reference Algorithm for Anomaly Localization uing MVTech Dataset<h1>
      <img src="Img/fau-logo-tech.png" width="300">
      <h2>Winter Semester 2020<h2>
  </div>
</div>

### Abstract
In applications like Medical Imaging, Traffic Surveillance and Industrial Product defects we need to detect and localize the anomalies. Few of the previous techniques depends on GMM and Deep learning techniques like VAE and GAN, thus involving anomalous training images to localize anomalies. Here in this project VAE-GAN is implemented, where VAE comprehends to localize the regions and retrives the image. Here GAN improves the image quality generated by VAE. The model is trained based on two different modes - unsupervised and semi-supervised mode. In Unsupervised mode, the model focuses on normal images so with given Anomalous image, the Convolutional Latent Variable preserves the abnormality and along with AdaCos similarity metric the model locates the anomaly. However, with Semi-supervised mode the model - trained with 1% anomalous image - prevents the model to make inference on normal region.
The final objective function is addition of VAE loss, adversarial loss and AdaCos loss.

The Project is dependent on the paper "Attention Guided Anomaly Localization in Images"

### Usage 
- `pip install mvtech_al` or 
- `git clone https://`

```python 
from torchsummary import summary
summary(your_model, input_size=(channels, H, W))
```

### Structure
```
|
+-- mvtech_al
|   | 
|   +-- main.py 
|   +-- *.py 
|   +-- *.py 
|   +-- *.py 
```