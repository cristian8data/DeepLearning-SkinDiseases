# System to support the diagnosis of chronic skin diseases
Rosacea and psoriasis are two chronic inflammatory skin diseases with similar facial symptons. 
This study focused on the search for predictive models for rosacea and psoriasis, using various 
architectures of Convolutional Neural Networks (CNNs) pre-trained through Transfer Learning.

## Authors
- [Cristian Morillo Losada](https://www.github.com/cristian8data)
- Alejandro Puente Castro
- Cristian Robert Munteanu

## Dataset
The images for this project were organized into two separate folders, each representing a different class: rosacea and psoriasis. The main dataset directory contained these class-specific folders:
- Rosacea (contains 56 images related to rosacea)
- Psoriasis (contains 60 images related to psoriasis)

## Installation
To run this project, it's necessary to install the following dependencies:

```bash
!pip install "torch==1.4" "torchvision==0.5.0"
!pip install fastai
```

## Environment Variables

The provided code initializes the environment and sets up some necessary variables and tools for working with the project:

```bash
import torch
torch.cuda.empty_cache()
!python --version
%reload_ext autoreload
%autoreload 2
%matplotlib inline

from google.colab import drive
drive.mount('/content/drive')
path = "/content/drive/MyDrive/Colab Notebooks/Images_folder"
```
The path specified in the code (`/content/drive/MyDrive/Colab Notebooks/Images_folder`) refers to the parent folder that contains both the "Rosacea" and "Psoriasis" folders. This allows the code to access the entire dataset, including both classes of images.

## License

[MIT](https://choosealicense.com/licenses/mit/)
