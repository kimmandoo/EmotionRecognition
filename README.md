# EmotionRecognition
## This repository is derived by [lampadovnikita's archive](https://github.com/lampadovnikita/EmotionRecognition)

This repository represents an android application performing recognition of facial emotions on an image.


### The parts that I changed..

- My project is written by Jetpack Compose and Kotlin only. 
- No GPU use, only cpu tensorflow lite
- Not firebase ml vision, It was changed to MLkit's FaceDetection API

|  |  |
|-|-|
|![image](https://github.com/user-attachments/assets/d9dcd153-85a9-40d2-84db-229a5175c0be)| <img src="https://github.com/user-attachments/assets/42d796db-5d86-499a-bfcb-afb0c1a45e1a" width="300">|

---
To train the CNN model there used hybrid dataset composed of the following datasets images:

- CK+ (all images except contempt images).
- JAFFE (all images).
- FER2013 (all images).
- RAF-DB (all images but only 205 happy class images).
  
The resulting hybrid dataset contains 46614 images and has the following data distribution:

All images was converted into the FER2013 images format - greyscale 48*48 pixels.

![image](https://github.com/user-attachments/assets/cfa64b8e-926e-49b9-bb6f-09b8bc502157)
