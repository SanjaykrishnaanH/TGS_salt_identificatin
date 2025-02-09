# TGS_salt_identificatin
To segment regions that contain salt from seismic images

# problem statement
Seismic data is collected using reflection _seismology, or seismic reflection_. The method requires a controlled seismic source of energy, such as compressed air or a seismic vibrator, and sensors record the reflection from rock interfaces within the subsurface. The recorded data is then processed to create a 3D view of earth’s interior. Reflection seismology is similar to X-ray, sonar and echolocation.<br>
<br>
A seismic image is produced from imaging the **reflection coming from rock boundaries**. The seismic image shows the boundaries between different rock types. In theory, the strength of reflection is directly proportional to the difference in the physical properties on either sides of the interface. While seismic images show rock boundaries, _they don't say much about the rock themselves_ ,some rocks are easy to identify while some are difficult.<br>
<br>
There are several areas of the world where there are vast quantities of salt in the subsurface. One of the challenges of seismic imaging is to identify the part of subsurface which is salt. Salt has characteristics that makes it both simple and hard to identify. **Salt density is usually 2.14 g/cc which is lower than most surrounding rocks**. The seismic **velocity of salt is 4.5 km/sec**, which is usually faster than its surrounding rocks. This difference creates a _sharp reflection at the salt-sediment interface_. Usually salt is an amorphous rock without much internal structure. This means that there is typically not much reflectivity inside the salt, unless there are sediments trapped inside it. The unusually high seismic velocity of salt can create problems with seismic imaging.<br>
<br>
# Dataset :
The data is a set of images chosen at **various locations chosen at random** in the subsurface. The images are 101 x 101 pixels and each pixel is classified as either **salt or sediment**. In addition to the seismic images, the depth of the imaged location is provided for each image. The goal of the competition is to segment regions that contain salt.<br>
[link to dataset!](https://www.kaggle.com/c/tgs-salt-identification-challenge/)
<br>

# code explanation :
the complete code works on _**U_NET architecture**_ which is a subset of CNN(DL).<br>
follow the comments in ipynb to execute the code .

# sample images/output :
sample result on training image: 
![sample result on training image](/images/index-1.png)
<br>
sample result on validation image:
![sample result on validation image](/images/index-2.png)
