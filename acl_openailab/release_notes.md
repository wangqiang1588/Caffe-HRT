# Release Note
[![License](https://img.shields.io/badge/license-BSD-blue.svg)](LICENSE)

The release version is 0.3.0. You can download the source code from [OAID/CaffeOnACL](https://github.com/OAID/CaffeOnACL)

## Verified Platform :

The release is verified on 64bits ARMv8 processor

- Hardware platform : Rockchip RK3399 ([Firefly-RK3399 board](http://wiki.t-firefly.com/index.php/Firefly-RK3399))
- Software platform : Ubuntu 16.04<br>

## ACL Compatibility Issues :
There are some compatibility issues between ACL and Caffe Layers, we bypass it to Caffe's original layer class as the workaround solution for the below issues

* Normalization in-channel issue
* Tanh issue
* Softmax supporting multi-dimension issue
* Group issue

Performance need be fine turned in the future

# Issue Report
Encounter any issue, please report on [issue report](https://github.com/OAID/CaffeOnACL/issues). Issue report should contain the following information :

*  The exact description of the steps that are needed to reproduce the issue 
* The exact description of what happens and what you think is wrong 


## Release History
The Caffe based version is [793bd96351749cb8df16f1581baf3e7d8036ac37](https://github.com/BVLC/caffe/tree/793bd96351749cb8df16f1581baf3e7d8036ac37).


## CaffeOnACL Version 0.3.0 - Aug 26, 2017

Support Arm Compute Library version 17.06 with 4 new layers added

* Batch Normalization Layer
* Direct convolution Layer
* Locally Connect Layer
* Concatenate layer


## CaffeOnACL Version 0.2.0 - Jul 2, 2017

Fix the issues:

* Compatible with Arm Compute Library version 17.06
* When OpenCL initialization fails, even if Caffe uses CPU-mode,it doesn't work properly.



## CaffeOnACL Version 0.1.0 - Jun 2, 2017 
   
  Initial version supports 10 Layers accelerated by Arm Compute Library version 17.05 : 

* Convolution Layer
* Pooling Layer
* LRN Layer
* ReLU Layer
* Sigmoid Layer
* Softmax Layer
* TanH Layer
* AbsVal Layer
* BNLL Layer
* InnerProduct Layer