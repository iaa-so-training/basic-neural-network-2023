# Severo Ochoa Basic Neural Networks 2023
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/iaa-so-training/basic-neural-network-2023/HEAD)

SO Basics of Neural Networks 2023 school at the IAA-CSIC

Deep learning (DL) is a family of techniques widely used in multiple fields with excellent results. Unfortunately, due to its steep learning curve, its use is not as extended as desirable. Several domain-specific libraries have been developed to facilitate the use of these DL models with modest success. For the widespread adoption of these techniques, researchers should be able to design and use their own DL models. Image classification is one of the main problems in astrophysics. The de facto standard to tackle this problem is Convolutional Neural Networks (CNN), a concrete deep learning architecture. A good knowledge of this technique is essential for its proper application by researchers. These three sessions have been designed with a goal in mind: to gain confidence in using CNNs for image classification tasks.

The tutor of this school is Dr Francisco Eduardo Sanchez Karhunen (Universidad de Sevilla).

**Summary of Contents**

- Session 1: Deep Learning fundamentals
- Session 2: Convolutional Neural Networks fundamentals
- Session 3: Practical considerations in real-world CNNs

# Agenda

## Thursday, November 16

### Session 1 (9:30 → 12:00) Deep Learning fundamentals

Roots of deep learning techniques. Reasons for layer stacking. Role of weights and activation functions. Layer as a map between representation spaces. Model parameters. Basic structure for classification tasks. Network training as an optimization problem. Weight initialization techniques. Typical loss functions and optimizers. Learning-rate scheduling.

Hands-on lab: Build from scratch a basic multilayer neural network using the Tensorflow-2 library. Sequential mode of layer stacking. Model training to tackle a classical basic image classification problem.

### Session 2 (14:00 → 18:30) Convolutional Neural Networks fundamentals

Drawbacks of classical multilayer networks in image classification tasks. Human brain image handling. Convolutional layers: padding and stride. Types of pooling layer. Kernels for feature map extraction. Kernel stacking. CNNs as an extension of classical stacked layer models. Top layers in CNNs.

Hands-on lab. Build from scratch a basic CNN for image classification using the Galaxy10 dataset.

## Friday, November 17
### Session 3 (9:30 → 13:00) Practical considerations in real-world CNNs

Overfitting in CNNs. Techniques for overfitting reduction: data augmentation and drop-out. Types of data augmentation. Drop-out rates. Transfer learning: concept and usage. Top Pre-Trained models for image classification. Handling large image datasets: ImageDataGenerators.
Hands-on lab: Use of ImageDataGenerators combined with realistic folder structures in image classification problems. Inclusion of data augmentation in our preprocessing pipelines. Add drop-out layers to the CNN design in session 2. Use of transfer learning in a real situation.

# Installation instructions
You can manage the instalation with `conda` following these steps:

1. Make sure you have conda/mamba installed. You can follow the instructions in [Installing miniconda](https://droplets-spsrc.readthedocs.io/conda/#installing-miniconda).

2. In a terminal, go to your working directory and clone this repository:

```
git clone https://github.com/iaa-so-training/basic-neural-network-2023.git
cd basic-neural-network-2023
```

3. Install the dependencies for the tutorials (replace `mamba` with `conda` if you don't have mamba installed):
```
mamba env create -f environment.yml
```

4. Execute the tutorials

You need to activate the conda environment and initialize a Jupyter Lab session:

```
conda activate iaa_nn
jupyter lab
```

Once everything is installed, you just need to run step 4 to run the tutorials.

You can also launch the tutorials without installation in the free myBinder service by clicking here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/iaa-so-training/basic-neural-network-2023/HEAD). Note that this is a free service with limited resources, useful to execute and modify the tutorials live, but computationally expensive steps may not be possible.


# Organizing Committee 

- Rainer Schödel (Chair), IAA-CSIC, Spain 
- Laura Darriba, IAA-CSIC, Spain  
- Javier Moldón, IAA-CSIC, Spain 


--- 
This event is supported by the "Center of Excellence Severo Ochoa" award to the Instituto de Astrofísica de Andalucía. We acknowledge financial support from the Severo Ochoa grant CEX2021-001131-S funded by MCIN/AEI/ 10.13039/501100011033 from the Instituto de Astrofísica de Andalucía.
