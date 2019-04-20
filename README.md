# prosthetics-mocap
A Proof of concept on how Prosthetics can be improved with the help of Motion capture and Machine learning Algorithms

The Idea behind this project is to demonstrate how existing Prosthetics can be improved by using IMU motion capture and Machine learning. 

IMU mocap[Motion capture] captures the human motion in a cartesian co-ordinate plane which is represted by 4 dimensions X,Y,Z and the 4th dimension is time. Based on these information, IMU's can help us track human motions and visualize them in 4 dimensions. 

In this project we have used the motion capture data in a c3d format as this format is predominantly used in forms of Gait analysis. 

For more information on c3d:
https://www.c3d.org/

Download Mokka here [https://biomechanical-toolkit.github.io/mokka/] to visualize the c3d files in a more easier way. 


The Data was taken from CMU[Carnegie Mellon University Motion Capture Database]  http://mocap.cs.cmu.edu/ 

This project is very experimental and will be updated and refined by trying with even more mocap samples and with different machine learning algorithms with more optimisations. 

The current Version of this project was done using XGBoost algorithm. Currently LSTMS are being tested out and will be updated shortly. 

Currently, The programming language of choice is R. I am also planning to replicate it in python as well with GPU support. 



Perspective View of the Prediction of File name 02_02 under subject 1 

![Alt Text](https://i.imgur.com/vxLWzP5.gif)

Orthogonal View of the Prediction of File name 02_02 under subject 1 

![Alt Text](https://github.com/Yogge-Yooge/prosthetics-mocap/blob/master/02_02_predicted_orthogonal_n1.gif)


Actual Skeleton view of the Motion 

![Alt Text](https://i.imgur.com/T5JPKtH.gif)

Machine Learning Methodology:- 
In this project, we are validating the human motion by testing around 97 sample c3d files and validating it on the 98th sample. 
The co-ordinates of the right side markers and the center markers of the body is used to predict the markers of the left side. 

Link to the dataset that has been used in this project dataset :- https://drive.google.com/open?id=1P4JEwggtCG7fT484ajxs0L9nW-EBwoqN 
