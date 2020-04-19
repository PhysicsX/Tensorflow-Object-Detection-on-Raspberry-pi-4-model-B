# Tensorflow-Object-Detection-on-Raspberry-pi-4-model-B


	cd Desktop/
	mkdir tensorflowRasp
	cd tensorflowRasp/
	python3 -m pip install virtualenv
	virtualenv env
	-> logout
	cd Desktop/tensorflowRasp/
	virtualenv env
	source env/bin/activate
	sudo apt-get install -y libhdf5-dev libc-ares-dev libeigen3-dev gcc gfortran python-dev libgfortran5 libatlas3-base libatlas-base-dev libopenblas-dev libopenblas-base libblas-dev liblapack-dev cython openmpi-bin libopenmpi-dev python3-dev
	sudo pip3 install keras_applications==1.0.8 --no-deps
	sudo pip3 install keras_preprocessing==1.1.0 --no-deps
	sudo pip3 install pybind11
	sudo pip3 install h5py==2.9.0
	sudo pip3 install -U six wheel mock
	wget https://github.com/lhelontra/tensorflow-on-arm/releases/download/v2.1.0/tensorflow-2.1.0-cp37-none-linux_armv7l.whl
	python3 -m pip install tensorflow-2.1.0-cp37-none-linux_armv7l.whl 
	-> logout
	cd Desktop/tensorflowRasp/
	source env/bin/activate
	python3
	-> import tensorflow
	sudo pip3 install pillow lxml jupyter matplotlib cython
	sudo apt-get install libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev libavcodec-dev libavformat-dev libswscale-dev libv4l-dev libxvidcore-dev libx264-dev qt4-dev-tools
	sudo pip3 install opencv-python
	python3
	-> import cv2
	pip3 install opencv-contrib-python==4.1.0.25
	python3
	-> import cv2
	sudo apt-get install protobuf-compiler
	protoc --version
	git clone --depth 1 https://github.com/tensorflow/models.git
	sudo nano ~/.bashrc
	export PYTHONPATH=$PYTHONPATH:/home/pi/Desktop/tensorflowRasp/models/research:/home/pi/Desktop/tensorflowRasp/models/research/slim
	cd models/research/
	protoc object_detection/protos/*.proto --python_out=.
	wget http://download.tensorflow.org/models/object_detection/ssdlite_mobilenet_v2_coco_2018_05_09.tar.gz
	tar -xzvf ssdlite_mobilenet_v2_coco_2018_05_09.tar.gz
	sudo apt-get install python3-picamera
	sudo pip3 install matplotlib
	pip install Pillow
	wget https://raw.githubusercontent.com/PhysicsX/Tensorflow-Object-Detection-on-Raspberry-pi-4-model-B/master/ObjectDetectionPiCamera.py?token=ABZJOAV7GBFOY4JFPTN6K526TR2NM
  
  change the file /home/pi/Desktop/tensorflowRasp/models/research/object_detection/utils/label_map_util.py
line 138 ->   with tf.io.gfile.GFile(path, 'r') as fid:
