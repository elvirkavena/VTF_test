# CV Test Task



## Task

The task is to capture faces from the camera, taking a photo every 1-5 seconds


#### requirements

```bash
pip3 install tensorflow==1.15.2
pip3 install numpy 
pip3 install scipy 
pip3 install opencv-python 
pip3 install pillow 
pip3 install matplotlib 
pip3 install h5py 
pip3 install keras 
pip3 install https://github.com/OlafenwaMoses/ImageAI/releases/download/2.0.2/imageai-2.0.2-py3-none-any.whl
```

## Solution

The task is consist of 3 parts:
1. Capture faces from the web camera
2. Take a photo every 1-5 seconds
3. If the face is known, show the name of the person

I solved the first and second problems. 

I chose OpenCV to recognize faces from the camera. I also tried imageai detection but did not get a good result.
I used Cascade classifier for face recognition which is "haarcascade_frontalface_default.xml":
```bash 
cascPath = "./haarcascade_frontalface_default.xml"
faceCascade = cv2.CascadeClassifier(cascPath)
```
 To capture faces from web camera I used this:
```bash
camera = cv2.VideoCapture(0)
```




