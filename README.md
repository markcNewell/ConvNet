# ConvNet
A Python implementation of ConvNet landmarks as detailed by:<br>
```Suenderhauf, Niko, Shirazi, Sareh, Jacobson, Adam, Dayoub, Feras, Pepperell, Edward, Upcroft, Ben, & Milford, Michael (2015) Place recognition with ConvNet landmarks: Viewpoint-robust, condition-robust, training-free. In Hsu, D (Ed.) Robotics: Science and Systems XI. Robotics: Science and Systems Conference, http://www.roboticsproceedings.org/, pp. 1-10.```

Designed to be used like OpenCV detection algorithms:<br>
```python
Import ConvNet
convnet = ConvNet.ConvNet()
des1, kp1 = convnet.detectAndCompute(image1)
des2, kp2 = convnet.detectAndCompute(image2)


score, matches = ConvNet.matchFeatures(des1, kp1, des2, kp2)


ConvNet.drawMatches(image1, kp1, image2, kp2, matches)
```
