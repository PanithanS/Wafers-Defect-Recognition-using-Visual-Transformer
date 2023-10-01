# Visual transformer for mixed-type wafer defect pattern recognition

Semiconductor manufacturing is a highly complex and precise process with numerous steps involved in creating integrated circuits on silicon wafers. Defects can occur at any stage of this process, from wafer fabrication to packaging. These defects can lead to yield loss and impact the performance of the final electronic devices. Manufacturers need to control the quality of semiconductor wafers to maintain high yields and reduce production costs.

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor--Manufacturing/assets/83627892/3e059907-fb2b-4ce9-8cbd-440e5afccb10)

## Context
Wafers defect pattern recognition (DPR) in semiconductor manufacturing is an essential step to inspect the defect pattern that can occur during the production of semiconductor wafers. DPR is not only about defect detection but also about understanding the root causes of defects. This coworking between DPR and defect root causes analysis is essential for semiconductor manufacturers to enhance their production, minimize defects, and boost yield, resulting in significant cost savings and the production of higher-quality semiconductor products. Deep learning for computer vision techniques is often employed to address the challenges of DPR in semiconductor manufacturing. These techniques leverage data from wafer maps, including spatial information, to train models capable of accurately detecting and classifying defects. However, defects can exhibit various spatial characteristics, such as size, shape, and distribution, and sometimes the presence of multiple defect types on a single wafer is even more complicated for defect identification and classification. Therefore, this requires an effective DPR system to handle mixed types of defects present on wafers.

## Dataset: MixedWM38
Here we use the dataset from https://github.com/Junliangwangdhu/WaferMap.
MixedWM38 Dataset(WaferMap) consists of 38000 wafer maps, including 1 normal pattern, 8 single defect patterns, and 29 mixed defect patterns, a total of 38 defect patterns.

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor-Manufacturing/assets/83627892/cfaaa855-0cf4-442a-8c19-10322361ee6d)

## Results

### Visual transformer (ViT) model
- The visual transformer divides the image into 4x4 patches and then applies a linear projection to these patches before encoding them into the dense layer. Next, the dense layer is combined with position embeddings and passed to the transformer block. These position-encoded features are further passed to a multilayer perceptron to generate an output prediction.

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor-Manufacturing/assets/83627892/cd9f6527-e2dc-4411-89c1-8b5988cb321f)

### Training and validation
- The training takes time depending on your computational power, however, the accuracy and loss may not be very different
- Here, we achieved an accuracy of 98.98% and a low loss value

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor-Manufacturing/assets/83627892/d30b5bbc-cb8a-4605-bdc0-ecafeda91c9f)

### Predictions
- The model performance looks acceptable.

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor-Manufacturing/assets/83627892/854feccc-df21-45ee-a962-1fb6e76bc849)

## Acknowledgements and inspirations
- We acknowledge the dataset provider for the Mixed-type Wafer Defect Datasets from the Institute of Intelligent Manufacturing, Donghua University
- See the dataset GitHub: https://github.com/Junliangwangdhu/WaferMap
- This work inspired from https://keras.io/examples/vision/image_classification_with_vision_transformer/

## Reference
1. J. Wang, C. Xu, Z. Yang, J. Zhang and X. Li, "Deformable Convolutional Networks for Efficient Mixed-type Wafer Defect Pattern Recognition," in IEEE Transactions on Semiconductor Manufacturing, DOI: 10.1109/TSM.2020.3020985.
2. Zheng, Xiaoqing, et al. "Recent advances in surface defect inspection of industrial products using deep learning techniques." The International Journal of Advanced Manufacturing Technology 113 (2021): 35-58.
3. Nag, Subhrajit, et al. "WaferSegClassNet-A light-weight network for classification and segmentation of semiconductor wafer defects." Computers in Industry 142 (2022): 103720.
4. Dosovitskiy, Alexey, et al. "An image is worth 16x16 words: Transformers for image recognition at scale." arXiv preprint arXiv:2010.11929 (2020).
