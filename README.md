# National-College-Student-s-innovation-and-entrepreneurship-training-program

## Automatic miniature bearing mechanical defect detection software and hardware integration system

## Objective.·
Bearing is an essential component in modern mechanical equipment; its primary function is to support the mechanical rotating body, reduce the friction coefficient during its movement, and ensure its rotary accuracy so that the quality and reliability of the bearing have highly demanding requirements.
Currently, to screen out the bearings that meet the requirements, the manual visual inspection method is generally used in industrial production. This is a high-cost and inefficient way of manual training. To address this pain point, we combine the current rapid development of image processing, pattern recognition, deep learning, and other related science to solve the interdisciplinary problem of "how to apply computer vision to industrial product inspection" and then form a set of "vision" link The feedback system can be used to improve the productivity and quality of industrial production by using the image inspection technology which is widely used in the automatic inspection of industrial products.

## Basic idea.
We designed a hardware and software system that can be used to detect bearing surface defects, through which the bearing surface defects can be accurately and automatically screened. The main steps are as follows: first (image acquisition), under the condition of coaxial illumination, the coaxial light image of the target bearing is acquired; under the condition of multi-angle and multi-light source illumination, the multi-light source image of the target bearing is acquired. Secondly (bearing localization), receive and process the coaxial optical image in the image acquisition module with the bearing center coordinates. Again (bearing region segmentation) reads the bearing center coordinates and divides the bearing into three different regions. Then (character recognition) reads the segmented center ring region of the image and uses the neural network to identify the trademark features. Finally (defect detection), receives the multi-angle light source image and identifies four defects (gaps, stains, flat caps, and scratches).

The main processing flow is shown in Figure 1.
![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/software%20component.png)


## Project progress.
First, we learned the circuit board principle and soldering method for hardware. To solve the problem of poor robustness and low efficiency of the previous generation of robot arm-based system, we soldered out the circuit board to control the six-way servo system. After preliminary experiments, the system’s efficiency was improved by 67% based on the original one. The third generation of the detection process system controlled by a microcontroller was initially completed with a six-servo model to accelerate the efficiency of the original hardware process system, and experiments were conducted. The specific process is shown in Figure 2.

![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/workflow.png)

In communication devices, millimeter wave (mmWave) communication is integrated into the hardware and software integrated system to increase the data transmission rate. In this system, we introduced low-complexity analog/digital hybrid precoding for signal processing. Hybrid precoding involves a combination of analog and digital processing, improving efficiency to support more data transmission to meet explosive communication demands.

On the software side, the overall software detection process is improved. In the case of text recognition, the original learning method is replaced, and MMORC is used for the distinction of bearing surface text for obtaining a sizable data set. We have implemented each algorithm module using a unified framework and modular design to achieve code reuse as much as possible. We abstracted the text detection, segmentation-based text recognition, and critical information recognition network structures into backbone, neck, head, and loss modules and the seq2seq text recognition network into the backbone, encoder, decoder, and loss modules. Various datasets were downloaded from the web to test the learning model.

We evaluated the overall hardware process, built a set of coaxial light sources using 3D printing (shown in Figure 3), and changed the human-machine interaction, i.e., the UI, according to today's hardware-software integration system.

![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/light.png)

## Research results and recent progress

1. We have actively participated in several national competitions within the university. In response to the competition, we drafted project plans, product plans and plans for future business ventures, and actively contacted relevant companies. Currently, we have won the first prize in the 17th Climbing Cup held in our school and achieved the fourth place. We have also actively participated in the provincial Challenge Cup and Internet Plus competitions and have gained a lot from these competitions.

![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/award.jpg)

2. In order to link soft and hard more closely together and improve the speed and stability of picture delivery, we introduced a signal processing system in the form of hybrid precoding. And based on this, we completed a paper on IoT communication, signal processing and delivery, which is currently being pitched at IPIC. In previous generations of software and hardware integration systems, we mainly used microcontroller serial communication to transmit the captured bearing pictures. We need to transfer 16 high pixel bearing pictures taken in 8 seconds to the software part for stitching and defect detection, but the efficiency cannot meet the requirements of fast industrial production process. To improve the data transfer rate, millimeter wave (mmWave) communication was integrated into the hardware and software integration system. To cope with the above mentioned problems, a low-complexity hybrid analog/digital precoding is introduced. The hybrid precoding involves the combination of analog and digital processing, which improves the efficiency to support more data transmission and meet the explosive communication demands. In addition, the implementation of wireless device communication frees our system from the problem of excessive data lines and overly heavy equipment. It is more portable and easy to install.

3. To learn various models and frameworks of adversarial neural networks in conjunction with the way of image processing in software processes, and to learn inter-image translation in this way, we propose to publish a research-based paper on the current adversarial neural networks in image translation. Currently EI is in the submission.
In addition, in the previous scheme, our detection results always received the effect of high light generated by illumination on the detection accuracy. In this study, based on the original neural network, we added the HA (highlight-aware) convolution operation, as shown in Figure 4, to repair the bearing images affected by high light. This convolution automatically learns a soft mask that represents the potentially overexposed region in the input image and uses it to weaken the invalid features generated by saturation. Weakening of invalid features generated by saturated pixels.

![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/HAA.png)

4. we achieved the previous phase of refinement of the overall construction goals
The next phase of the work is focused on the experimental aspect, obtaining the training set by image acquisition of the existing framework model. And in this way the learning model will be detected. In addition we will compare the detection efficiency and detection accuracy of the detection framework of this integrated system. Evaluate whether the new generation of detection process is more efficient than the original design by robotic arm flip.
In terms of the project, we are not bound to the concept of the product, the process designed out, but want to get a concrete product. To do this, we will study easier inspection methods as well as design an overall product framework. This is shown in Figure 5.

![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/hh1.jpg)
![main](https://github.com/wenyihan4396/National-College-Student-s-innovation-and-entrepreneurship-training-program/blob/main/hh2.png)












