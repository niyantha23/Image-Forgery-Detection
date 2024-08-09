# Digital Image Forgery Detection Using Pre-Trained Xception Model as Feature Extractor

**Author:** Niyantha Maruthu Pandiyan  
**Affiliation:** School of Computer Science and Engineering, Vellore Institute of Technology, Vellore, India  
**ORCID:** [0000-0002-5375-9411](https://orcid.org/0000-0002-5375-9411)

## Abstract

With the proliferation of digital images on the internet and advancements in image editing software, tampering with original images has become increasingly easy. This paper presents a Deep Learning approach for detecting fake or altered images by utilizing a pre-trained Xception model as a feature extractor. The proposed method, trained on the CASIA-V2 dataset, achieves high accuracy in classifying images as tampered or real.

## Index Terms

Image Forgery Detection, Transfer Learning, Deep Learning, CNN, Feature Extraction, Xception

## Introduction

In the age of digital communication, images play a crucial role in conveying information and evidence. However, advancements in technology have made it easier to manipulate images, posing challenges for detecting such forgeries. This paper focuses on leveraging deep learning techniques to detect tampered images, specifically using a pre-trained Xception model for feature extraction.

## Methodology

### Architecture

The architecture comprises three main modules:
1. **Preprocessing:** Images are resized to 256x256 and undergo Error Level Analysis (ELA). Preprocessed images are then converted into numpy arrays and split into training, validation, and test sets.
2. **Feature Extraction:** A pre-trained Xception model extracts features from the images. Xception is chosen for its balance of accuracy and computational efficiency.
3. **Classification:** Features extracted by Xception are fed into a classification head consisting of global average pooling, two dense layers, and a softmax activation function to classify images as tampered or real.

## Experimental Results

### Dataset

The model is trained on the CASIA ITDE v2 dataset, which includes 7,200 authentic and 5,123 tampered images. Due to computational constraints, a subset of 1,200 authentic and 1,200 tampered images was used.

### Performance Metrics

The model achieved:
- **Accuracy:** 95% on the test set
- **True Positive Rate (TPR):** 98.2%
- **True Negative Rate (TNR):** 98.3%
- **False Positive Rate (FPR):** 1.6%

## Results Comparison

| Model                 | Accuracy |
|-----------------------|----------|
| Kuznetsov et al. [4]  | 97.8%    |
| Ortega et al. [8]     | 98%      |
| Walia et al. [7]      | 99.31%   |
| **Proposed Model**    | **95%**  |

## Conclusion and Future Work

The proposed deep learning model effectively classifies images as authentic or tampered using a pre-trained Xception model. While achieving a 95% accuracy, further improvements can be made by utilizing the full CASIA v2 dataset and exploring other feature extraction methods.

## References

1. H. D. Deng, “Image Level Forgery Identification and Pixel Level Forgery Localization via a Convolutional Neural Network,” 2018.
2. A. Doegar, M. Dutta, and G. Kumar, “CNN based Image Forgery Detection using pre-trained AlexNet Model,” Proc. Int. Conf. Comput. Intell. IoT 2018, pp. 402–407, 2018.
3. J. H. Bappy et al., “Hybrid LSTM and Encoder-Decoder Architecture for Detection of Image Forgeries,” IEEE Trans. Image Process., vol. 28, no. 7, pp. 3286–3300, 2019.
4. A. Kuznetsov, “Digital image forgery detection using deep learning approach,” J. Phys. Conf. Ser., vol. 1368, no. 3, 2019.
5. [Additional references here]

