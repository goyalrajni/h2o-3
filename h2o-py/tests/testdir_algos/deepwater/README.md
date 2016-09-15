# Deep Water Python Tests

### What can Deep Water do?
* Train user-defined or pre-defined deeplearning models for image classification
* Train on a single GPU (requires CUDA) or CPU (requires BLAS) 
* Uses the MXNet backend transparently
* Behave just like any other H2O model (Flow, cross-validation, early stopping, hyper-parameter search, etc.)

### Image Classification Toy Dataset used
https://h2o-public-test-data.s3.amazonaws.com/bigdata/laptop/deepwater/imagenet/cat_dog_mouse.tgz

### To run examples:
* Install CUDA 8
* Install CUDNN 5
* Obtain GPU-enabled h2o.jar (currently H2O-internal only, in testing)
* Run with `CUDA_path=/usr/local/cuda java -jar h2o.jar`
* Download dataset above (unpack contents into directory ./bigdata/laptop/deepwater/imagenet/<here>, relative to where h2o was launched)
* Run python tests with `python ./pyunit_lenet_deepwater.py`