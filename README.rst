"Exact Information Bottleneck with Invertible Neural Networks: Getting the Best of Discriminative and Generative Modeling" (2020)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

https://arxiv.org/abs/1907.02392

USAGE
^^^^^^^^^^^^^^

* All configuration files for all experiments in the paper are contained
  in the directory 'experiments_configs'.

* Training (for one example configuration):

      `python -W ignore main.py train experiments_configs/cifar10/full_model.ini`

* Testing:

      `python -W ignore main.py test experiments_configs/cifar10/full_model.ini`

* The cifar/mnist datasets should be downloaded automatically the first time
  it is run. For the OoD evaluation, tiny imagenet and quickdraw have to be downloaded
  separately.

REQUIREMENTS
^^^^^^^^^^^^^^

To implement the INNs, we use of the FrEIA library
(github.com/VLL-HD/FrEIA)

.. code:: sh

    pip install git+https://github.com/VLL-HD/FrEIA.git

Additional requirements:

* pytorch=1.4.0
* numpy=1.18.1
* matplotlib=3.1.3
* torchvision=0.2.2
