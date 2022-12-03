# National-College-Student-s-innovation-and-entrepreneurship-training-program

## Automatic miniature bearing mechanical defect detection software and hardware integration system

## Objective.·
Bearing is an essential component in modern mechanical equipment; its primary function is to support the mechanical rotating body, reduce the friction coefficient during its movement, and ensure its rotary accuracy so that the quality and reliability of the bearing have highly demanding requirements.
Currently, to screen out the bearings that meet the requirements, the manual visual inspection method is generally used in industrial production. This is a high-cost and inefficient way of manual training. To address this pain point, we combine the current rapid development of image processing, pattern recognition, deep learning, and other related science to solve the interdisciplinary problem of "how to apply computer vision to industrial product inspection" and then form a set of "vision" link The feedback system can be used to improve the productivity and quality of industrial production by using the image inspection technology which is widely used in the automatic inspection of industrial products.

## Basic idea.
We designed a hardware and software system that can be used to detect bearing surface defects, through which the bearing surface defects can be accurately and automatically screened. The main steps are as follows: first (image acquisition), under the condition of coaxial illumination, the coaxial light image of the target bearing is acquired; under the condition of multi-angle and multi-light source illumination, the multi-light source image of the target bearing is acquired. Secondly (bearing localization), receive and process the coaxial optical image in the image acquisition module with the bearing center coordinates. Again (bearing region segmentation) reads the bearing center coordinates and divides the bearing into three different regions. Then (character recognition) reads the segmented center ring region of the image and uses the neural network to identify the trademark features. Finally (defect detection), receives the multi-angle light source image and identifies four defects (gaps, stains, flat caps, and scratches).

The main processing flow is shown in Figure 1.
![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/software%20component.png)
