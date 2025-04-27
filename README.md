**Parking Space Counter**

In this project, we create a Parking Space Counter using basic image processing techniques with OpenCV.
The system detects how many parking spots are occupied and how many are free in a given parking lot video.

# Demo

![image](https://github.com/user-attachments/assets/c659ff5b-ad67-4d6c-b7d6-28b64a87d516)

#Project Overview
* Video Input: A prerecorded video (carPark.mp4) of a parking lot.
* Parking Spot Detection: Manually mark parking spots on a static image (carParkImg.png) and save the coordinates.
* Occupancy Detection:
  -Convert frames to grayscale.
  -Apply Gaussian Blur and Adaptive Thresholding.
  -Dilate the image to enhance parking space features.
  -Count non-zero pixels in each parking spot to determine if it's occupied or free.
* Output:

  -Green rectangle => Free space.
  -Red rectangle => Occupied space.
  -Live counter showing available spots.

**Technologies Used**
-Python 3
-OpenCV
-cvzone (for easier text and rectangle drawing)
-Pickle (for saving/loading parking spot positions)
-NumPy
