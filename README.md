# An-Automatic-Attendance-System-Based-on-Face-Recognition
An Automatic Attendance System Based on Face Recognition and Covid-19 Health Conditions via Deep Learning



Maintaining the attendance is essential in every educational institution for checking
the performance of students. Taking attendance using traditional methods wastes
time due to the high capacity of students, which makes the educational system less
effective. To address this, our proposed project, a complete system that automates
attendance taking using face recognition, allows easy access to attendance records in
one location. It also recognizes Tawakkalna status automatically by scanning the QR
code without human involvement and measures temperature to ensure the health and
safety for students.



## Normally, four phases constitute of the facial recognition technique:
1. Facial detection
2. Face standardization
3. Extraction of feature
4. Facial identification and verification

![Picture1](https://user-images.githubusercontent.com/67114907/147417194-ada337b3-9690-44e7-a6c6-7c138a797468.jpg)


## Face Recognition System
Face recognition is utilized in which the program can detect the face of a person using a camera and identify the individuals from the data set (supervised learning). To detect the face place, it puts a square box and label the name of the person on the box to identify him. We used Face recognition library which is called OpenCV. On this library, we made the program to open the camera and look at the person live by making a loop for each frame and when it is done fast it shows as a live video.LBP function was utilized from openCV library to perform the most important part of the implementation as shown below ..



### Face Recognition with OpenCV and Local Binary Patterns 
![Picture2](https://user-images.githubusercontent.com/67114907/147417385-f2193fee-b77b-4aca-bc18-8c61bf3f21ca.png)

Local Binary Patterns (LBPs) for face recognition algorithm will be discussed, as well as how it works. LBPs are implemented in OpenCV, in the scope of face recognition. Considering a dataset containing a face, the first step is to split the face into 7 by 7 equal-sized cells as shown in Fig. Then Local Binary Pattern histogram is generated for each cell. A histogram, by definition, discards any location data about how the patterns are arranged adjacent with each other. But, by generating a histogram for each cell, we are able to store a degree of locative knowledge such as the mouth, nose, eyes, and so on.
This locative encoding also enables us to weight the histograms produced by each of the measured cells uniquely, offering greater characteristic strength to more distinctive facial characteristics.

The initial facial picture has been separated into 7 by 7 cells (left Fig.). The weighting system for each cell is then shown (Right Fig.):
![Picture3](https://user-images.githubusercontent.com/67114907/147417412-56b66a8e-963a-4516-ab34-0be671f7d33a.png)

    •	White cells (i.e., the eyes) are weighted 4 times higher in LBP histograms than other remaining cells. 

    •	The contribution of light gray cells (i.e., mouth and ears) is twice higher than that of gray cells.


    •	The contribution of dark gray cells is just 1.

    •	Finally, dark cells (i.e., the nose and cheek )are ignored and given a weight of 0.
Ahonen et al. discovered these weighting ratios by using hyperparameter tuning techniques to their training data, and testing data sets. Finally, the resulting feature vector is created by combining the loaded 7 by 7 LBP histograms.


### Project demo
https://youtu.be/FySJQzA0adI
by Zohair Tahhan
