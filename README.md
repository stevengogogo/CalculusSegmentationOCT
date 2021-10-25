# Calculus Segmentation from OCT imaging with U-Net 

![Segmentation](https://user-images.githubusercontent.com/29009898/138654388-de9c0959-3c6f-4fb7-a59a-dafc4b981023.png)
> Dental calculus segmentation with U-Net (test set)


## Why detecting dental calculus is hard?

Calculus formation is not always observable from the surface. This is a major obstacle to the early treatment of dental caries. Though X-ray is a standard tool for evaluating caries prognosis, **the biofilm-formed calculus can be hardly detected**. Furthermore, eye observation is limited to the surface, ignoring **subgingival calculus** that is the major cause of periodontitis. 

## How Optical coherence tomography (OCT) can improve the diagnosis?

|![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/OCT_B-Scan_Setup-en.svg/375px-OCT_B-Scan_Setup-en.svg.png)|![image](https://user-images.githubusercontent.com/29009898/138658467-32f467a5-1e38-4396-b00a-bd85404d2b9e.png)|
|---|---|
> Image source: Schneider, Hartmut, et al. 2017

Optical coherence tomography (OCT) provides a non-invasive way to observe calculus covered by the gingiva. The Fourier optic provides an adjustable focal plain that can visualize the calculus in the subgingival region with far-red light. It is also comparatively cheaper and possible to be portable in the near future.

## Why image processing is needed for OCT imaging?

However, OCT imaging is noisy and distorted by the reflection of the enamel. Although The human eye can observe the calculus region slice by slice, the automatic segmentation can provide a window for diagnosis. On the other hand, OCT is able to acquire 3D sections. 3D reconstruction provides a new era of periodontology in diagnosis and treatment evaluation. Therefore, automatic segmentation is required in this application.

## Why did I choose U-Net for automatic segmentation?

Due to sparse datasets and distorted images, U-Net provides a robust tool for primary data augmentation and high accuracy segmentation in small datasets. The overall training performance is listed in the following table:

|Performance|Training|Testing|
|---|---|---|
|Dice score|98%|86%|

## Conclusion

U-Net is a promising way for the novel application of dental calculus detection via OCT imaging. We should acquire more labeled datasets and compare images under different material interference. 


## About dataset

- The original dataset is not uploaded in this repo, please contact Dr. Shyh‐Yuan Lee.
