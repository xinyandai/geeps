- replace cudnn with https://raw.githubusercontent.com/BVLC/caffe/master/include/caffe/util/cudnn.hpp
- edit Makefile.config and modify INCLUDE_DIRS
```
INCLUDE_DIRS := $(PYTHON_INCLUDE) /usr/local/include /usr/include/hdf5/serial 
```
- hdf5 in ubuntu, the location of hdf5.so is can be found with ```dpkg -L libhdf5-dev```
```
LIBRARY_DIRS := $(PYTHON_LIB) /usr/local/lib /usr/lib /usr/lib/x86_64-linux-gnu/hdf5/serial/
```
- opencv3.2 not compatible with opencv4
- edit Makefile.config and uncomment to use `pkg-config` to specify OpenCV library paths.
```
USE_PKG_CONFIG := 1
```
 
