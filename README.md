
Install Python 3.7
Install Conda
update graphic card driver using NVIDIA experience
**using the Anaconda Prompt in administrator mode
**while in the Anaconda Prompt

$ conda create --name tf_gpu tensorflow-gpu 
$ conda install -c menpo opencv
$ conda create -n tf tensorflow

**then install all the missing package you need, for that time:

$ https://pjreddie.com/darknet/install/
$ conda install -c conda-forge imutils 
$ pip install -U scikit-learn scipy matplotlib
$ pip install scikit-learn==0.22.2
$ pip install filterpy


after we install these, try

$ cd C:\Users\QWER\AppData\Local\Programs\Python\Python36\YOLO\Counter\python-traffic-counter-with-yolo-and-sort-master

$ python main.py --input input/1.0.mp4 --output output/highway.avi --yolo yolo-coco

