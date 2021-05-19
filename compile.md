- replace cudnn with https://raw.githubusercontent.com/BVLC/caffe/master/include/caffe/util/cudnn.hpp
- edit Makefile.config and modify INCLUDE_DIRS
```
INCLUDE_DIRS := $(PYTHON_INCLUDE) /usr/local/include /usr/include/hdf5/serial 
```
