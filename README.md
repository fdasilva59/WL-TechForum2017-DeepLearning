# WL-TechForum2017-DeepLearning

This project contains the Jupyter notebooks from the Deep Learning talk we gave with Julien Carme for the Worldline 2017 TechForum. The aim of these 3 notebooks is to provide a short introduction to Tensorflow and Keras 



## How to install

- Install Ubuntu 14.04 LTS in a Virtual Machine (depending on your system)
- Install conda on your system ( https://conda.io/miniconda.html ) 

- update conda, create a  Python 3 environment, install Tensorflow 1.0.1 and keras :
```
conda update conda
conda create --prefix  ~/DataScience python=3.6 scipy numpy numba matplotlib pandas ipython jupyter sympy nose scikit-learn bokeh tensorflow 
source activate ~/DataScience
pip install --ignore-installed --upgrade https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-1.0.1-cp36-cp36m-linux_x86_64.whl
pip install keras
```	

Change your current directory to the one where you have cloned the notebooks; and start Jupyter notebook :
```
jupyter notebook --no-browser > /tmp/jupyter.log 2>&1 &
```

You can then open Jupyter in a web browser at " http://127.0.0.1:8888/tree " (Use a browser like Chromium inside you VM or don't forget to redicet port 8888 (Jupyter) and 6006  (Tensorboard) if you are accessing Jupyter in a VM from your host computer's browser)

## Note 

The first 2 notebooks are ok to be used in a VM on a laptop with only cpu such as a Intel core i5

It is however advised to use a GPU configuration (AWS or Floydhub) to execute the third notebook. On a laptop with core i5, it takes +45min to train on the CPU, whereas it takes less than 2 minutes on a server with a Nvidia K80 GPU


## Copyrights

These notebooks are inspired from Tensorflow and Keras Tutorials and are using the MNIST dataset. See : 

- www.tensorflow.org
- www.keras.io
- http://yann.lecun.com/exdb/mnist/
- https://www.tensorflow.org/get_started/mnist/beginners
- https://github.com/fchollet/keras/blob/master/examples/mnist_mlp.py
- https://github.com/fchollet/keras/blob/master/examples/mnist_cnn.py






