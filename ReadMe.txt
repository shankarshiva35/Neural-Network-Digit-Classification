Artificial Neural Network for Digit Classification.

***System Architecture***
Python 2.7


***External Libraries***
1) Numpy
2) python-mnist


***Installation***
Run the following command:

For Ubuntu:-
--> sudo pip install -r requirements.txt

For Windows:-
--> C:\Python27\Scripts\pip.exe install -r requirements.txt

(Please follow this link: https://github.com/BurntSushi/nfldb/wiki/Python-&-pip-Windows-installation
to install software from pip in Windows if you have trouble)

If you have trouble installing the software please follow the instruction guide in below links:

For Numpy:-
--> https://docs.scipy.org/doc/numpy-1.10.0/user/install.html

For python-mnist
--> https://github.com/sorki/python-mnist#installation

***DataSet***

Test Data is present in "data" folder. Need to download training dataset as follows

Download two dataset files from the following link : http://yann.lecun.com/exdb/mnist/
1) train-images-idx3-ubyte.gz:  training set images (9912422 bytes)
2) train-labels-idx1-ubyte.gz:  training set labels (28881 bytes)

Once downloaded, extract it and save it in the directory name "data" in the project folder.
File names must be following for the images and lables file respectively.
1) train-images-idx3-ubyte
2) train-labels-idx1-ubyte

***Running the code***

Testing:
--> python neuralnet.py

Training (Approximate 5-7 minutes):
--> python neuralnet.py --training

Testing with dropout rate (e.g. dropout rate=0.2):
--> python neuralnet.py -d 0.2

Training with dropout rate (e.g. dropout rate=0.2):
--> python neuralnet.py --training -d 0.2

Testing on different data set (trainSet, validationSet, testSet):
For e.g. the following command evaluates the network on the test dataset.
--> python neuralnet.py -t testSet

Help. Please use the following command to see full set of arguments and operations.:
--> python neuralnet.py --help