# install-instruction-for-YOLO

I try different installation method, the following step can make YOLO work under Win10

•	Install Python 3.6.6
•	Install Conda
•	Install the graphic card driver: using NVIDIA experience(dont search your driver derictly on google, NVIDIA experience can automaticlly detect your card model and install the right one for you)
•	clone https://github.com/thtrieu/darkflow, download necessary .cfg and weights from https://pjreddie.com/darknet/yolo/
•	conda create -n darkflow-env python=3.6
•	activate darkflow-env
•	pip install tensorflow-gpu
•	conda install cython numpy
•	conda config --add channels conda-forge
•	conda install opencv
•	conda install tensorflow-gpu (some times the pip install tensorflow-gpu doesnt install the CUDA properly, so use the conda again )
•	cd to the path of the YOLO folder (still using the Anaconda Prompt)
•	python setup.py build_ext –inplace
•	python flow --model cfg/yolo.cfg --load bin/yolov2.weights --demo videofile.mp4 --saveVideo --gpu 0.7 

Run your own script:
open cmd window
cd to the YOLO folder
activate darkflow-env
python videoFile.py

My conputer cfg:
Core i5 7th + GTX 1050ti + 8Gb RAM
the FPS is about 25 FPS
see the example on youtube:https://youtu.be/PpI4r2vID8I
