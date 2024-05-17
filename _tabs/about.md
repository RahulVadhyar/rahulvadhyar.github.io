---
# the default layout is 'page'
icon: fas fa-info-circle
order: 4
---
<hr>

## Introduction

Hi, I am Rahul Satish Vadhyar, a passionate Machine learning enthusiast that likes to train big and complex models. Besides that, I also am interested in computer graphics and operating systems.
Currently I am a 3rd year engineering student at BMS College of Engineering pursuing my B.E. in Artificial Intelligence and Machine Learning.

Over the years, I have picked up a solid understanding of the basics of Machine Learning and Deep learning and hvae gained experience in using various frameworks and libraries such as tensorflow and pytorch. I also take interest in computer graphics and have knowledge in Vulkan, GLFW, OpenGL, and GLSL.

Apart from my college studies, I have done an internship at Crowd Wisdom Trading for 11 months and have passed the official Tensorflow developer certification exam in 2022. I have done many projects such as Scene Understanding,
Don't Slouch, Hilichurl to English Translator, Pet Emotion Detection and Replication in Metaverse etc. 

Personally, I daily drive Fedora Linux with the KDE Plasma desktop environment. When I am free, I tend to work on my projects or learn new things. I also like to rice (customize) my desktop and make it look good.

<hr>

## Education:
![](assets/img/bmsce.jpeg){: w = "50", h = "50", .left}
<h4>
B.E. in Artificial Intelligence and Machine Learning, BMS College of Engineering, Bangalore. (2021 - current)
</h4>

I am currently in 6th semester of my engineering course. It is due to be completed by 2025. 

Some of the courses taken include Data Structures, Design and Analysis of algorithms, Database Management Systems,
Operating Systems, Introduction to Artifical Intelligence, Mathematical Foundations for Machine Learning, Linear
Algebra, Probability and Statistics for Machine Learning.

<hr>

## Certifications:
I have passed the official Tensorflow developer certification exam in 2022.
![Tensorflow Certificate](https://api.accredible.com/v1/frontend/credential_website_embed_image/certificate/56236386)

<hr>

## Internship:

I have done an internship at Crowd Wisdom Trading for 11 months. I prototyped an automated day trading system using reinforcement learning.

<hr>

## Programming Languages:
I am proficient in the following programming languages:
- Python
- C++
- C

<hr>

## Skills and Tools:

I have been involved in machine learning and deep learning since 2022, and have also gained experience in the following tools

- Tensorflow (officially certified since 2022) :  This is the first deep learning library I learned and I have used it in many projects. I also used it during my internship at Crowd Wisdom Trading.


- Pytorch : Recently, I have started using PyTorch more. I found that transformers were easier and more efficient to implement in PyTorch. Hence, recently, almost all my projects are using PyTorch.


- Git : For managing my projects and collaborating with others, I use Git. I find it to be an essential tool for all my projects to keep track of changes and maintain a history of my projects along with safe backups.


- SQL : I have used SQL in my Database Management Systems course and have been practicing it since then.

Apart from this, while working on my Chronos project, I have also gained experience in computer graphics and Vulkan, GLFW, OpenGL, and GLSL.

<hr>

## Projects

### Chronos(Under Development)

This is a 2D game engine that I am developing. It is written in C++ and uses Vulkan for rendering. It is a project that I am working on to learn more about computer graphics and game development.
I designed this engine to be easy to use and have a simple API. It was mainly created for me to develop a 2D side scroller game which I wanted to make. Development of the engine is still in progress and I am adding more features to it and fixing bugs. But hopefully, I will be able to complete it soon. Right now the codebase is around 5K lines of code. Below is a screenshot of the engine in action.

![](assets/img/chronoseditor.png)

Some of the advanced features it includes are:
- Efficient Rendering using Vulkan.
- Cross Platform support(Windows and linux(includes wayland and x11)).
- Easy to use GUI editor.
- Simple and easy to use API.
- Support for animations, which includes advanced features like skeletal animations, keyframe animations, etc.
- Support for Multi Sample Anti Aliasing(MSAA) and Anisotropic Filtering.
- Easy to debug with the comprehensive logging and debugging system.
- CI/CD integration with github actions for automated testing and deployment.
- Extensive documentation with a dedicated website developed using Doxygen.

[Github](https://github.com/RahulVadhyar/Chronos)  [Documentation](https://rahulvadhyar.github.io/Chronos/)

### Hilichurl to English Translator

This is a project that I worked with my friends on. Hilichurl is a mythical language in a popular game called Genshin Impact. The vocabulary of this language is less. Hence we took this challenge upon ourselves to make a translator that could translate this language to english. We accomlished this by creating a custom dataset consisting of around 1000 sentences. Then using PyTorch, we trained an advanced state of the art transformer to learn this language based on the dataset. Other notable things about this project include custom tokenizers for both english and Hilichurl that used the wordpiece tokenization algorithm. This was a huge contributor to the model's performance. 
A iOS app is being developed to use this model.

[Github](https://github.com/shrenisc/Hilichurlian-Eng)

### Don't Slouch
![Desktop View](https://github.com/RahulVadhyar/dontSlouch/blob/main/docs/Black%20White%20Elegant%20Monogram%20Initial%20Name%20Logo%20(1).png?raw=true){: w=10 h=10 .left}
Me and my friends developed this project during a hackathon that we won first place. This project was developed to help people maintain a good posture while working. It uses a webcam to detect the user's posture and gives feedback on it. We accomplished this by
collecting a small dataset of around 300 images. However due to the small size of the dataset, we performed extensive data augmentation and normalization techniques in order to improve the model's perfomance. The pipeline consists of using mediapipe to detect certain 
landmarks on the user and then using a small feedforward network with layernorm and dropout to classify the user's posture.\

### Scene Understanding

The objective of this project is to develop a contextual caption generator for images. The model takes an image as input and generates a caption that describes the image. The model is trained on the COCO dataset which consists of images and their corresponding captions. 
The model architecture is notable as it uses a custom transformer architecture along with a mobileViT feature extractor. The model is 72M parameters in size and took 72 hours to train on about 30GB of data. For easy user interaction, a simple GUI was developed using tkinter.

[Github](https://github.com/RahulVadhyar/SceneUnderstanding)

### Pet Emotion Detection and Replication in Metaverse


![Desktop View](assets/img/samsungcertificate.png){: w = "50", h = "50", .left}
This was a project that I along side my friends developed for Samsung under the PRISM program. The objective of this project was to detect the emotions of a pet using a webcam and then replicate the pet in the metaverse. We accomplished this by scraping a custom dataset from flickr. This dataset consisted of images of pets with their corresponding emotions. Total dataset turned out to be around 20K images. We then created a 3 model pipeline to detect, classify and extract the emotions of the pet. The models were trained using transfer learning on a pretrained EfficientNetB0 model with a custom head. This was then integrated with unreal engine that consisted of a VR environment where the pet was replicated. 

<hr>

## LeetCode:

Lately in order to improve my problem solving skills, I have started solving problems on LeetCode. My current progress is shown below:

![](https://leetcard.jacoblin.cool/Rahul58405u04)