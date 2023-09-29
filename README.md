# Visual transformer for mixed-type wafer defect pattern recognition

Semiconductor manufacturing is a highly complex and precise process with numerous steps involved in creating integrated circuits on silicon wafers. Defects can occur at any stage of this process, from wafer fabrication to packaging. These defects can lead to yield loss and impact the performance of the final electronic devices. Manufacturers need to control the quality of semiconductor wafers to maintain high yields and reduce production costs. Wafers defect pattern recognition (DPR) in semiconductor manufacturing in semiconductor manufacturing is an essential step to inspect the defect pattern that can occur during the production of semiconductor wafers. DPR is not only about defect detection but also about understanding the root causes of defects. Identifying the underlying reasons for defects helps in implementing corrective actions to prevent them from recurring.

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor--Manufacturing/assets/83627892/3e059907-fb2b-4ce9-8cbd-440e5afccb10)

## Wafers defect pattern recognition
Wafers defect pattern recognition (DPR) in semiconductor manufacturing in semiconductor manufacturing is an essential step to inspect the defect pattern that can occur during the production of semiconductor wafers. DPR is not only about defect detection but also about understanding the root causes of defects. This coworking between DPR and defect root causes analysis is essential for semiconductor manufacturers to enhance their production, minimize defects, and boost yield, resulting in significant cost savings and the production of higher-quality semiconductor products. 

## Deep learning solution and challenges
Deep learning for computer vision techniques is often employed to address the challenges of DPR in semiconductor manufacturing. These techniques leverage data from wafer maps, including spatial information, to train models capable of accurately detecting and classifying defects. However, defects can exhibit various spatial characteristics, such as size, shape, and distribution, and sometimes the presence of multiple defect types on a single wafer is even more complicated for defect identification and classification. Therefore, this requires a fast and accurate DPR system to handle mixed types of defects present on wafers.

## Dataset
Wafer map data, representing the locations of wafer defects and their patterns

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor-Manufacturing/assets/83627892/cfaaa855-0cf4-442a-8c19-10322361ee6d)

## Visual transformer (ViT)

### ViT model training and validation accuracy

![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor-Manufacturing/assets/83627892/d30b5bbc-cb8a-4605-bdc0-ecafeda91c9f)

## Results
![image](https://github.com/PanithanS/Wafers-Defect-Recognition-for-Semiconductor-Manufacturing/assets/83627892/854feccc-df21-45ee-a962-1fb6e76bc849)

## Acknowledgement and inspiration
- We acknowledge the dataset provider for the Mixed-type Wafer Defect Datasets from the Institute of Intelligent Manufacturing, Donghua University
- See the dataset GitHub: https://github.com/Junliangwangdhu/WaferMap
- This work inspired from https://keras.io/examples/vision/image_classification_with_vision_transformer/

## Reference
1. J. Wang, C. Xu, Z. Yang, J. Zhang and X. Li, "Deformable Convolutional Networks for Efficient Mixed-type Wafer Defect Pattern Recognition," in IEEE Transactions on Semiconductor Manufacturing, DOI: 10.1109/TSM.2020.3020985.
2. Zheng, Xiaoqing, et al. "Recent advances in surface defect inspection of industrial products using deep learning techniques." The International Journal of Advanced Manufacturing Technology 113 (2021): 35-58.
3. Nag, Subhrajit, et al. "WaferSegClassNet-A light-weight network for classification and segmentation of semiconductor wafer defects." Computers in Industry 142 (2022): 103720.
