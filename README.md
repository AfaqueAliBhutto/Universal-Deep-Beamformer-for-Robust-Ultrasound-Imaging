# Universal-Deep-Beamformer-for-Robust-Ultrasound-Imaging
Computer code and dataset for "Universal Deep Beamformer for Robust Ultrasound Imaging"

Paper
===============
* Shujaat Khan, Jaeyoung Huh, and Jong Chul Ye. "Universal Deep Beamformer for Robust Ultrasound Imaging." https://arxiv.org/abs/1901.01706v1.

Implementation
===============
* MatConvNet (matconvnet-1.0-beta24)
  * Please run the matconvnet-1.0-beta24/matlab/vl_compilenn.m file to compile matconvnet.
  * There is instruction on "http://www.vlfeat.org/matconvnet/mfiles/vl_compilenn/"
  * Please run the installation setup (install.m) and run some training examples.
 
Trained network
===============
* Trained network for 'Universal Deep Beamformer CNN' is uploaded.

Test data
===============
* Test data file is placed in 'data\cnn_sparse_view_init_multi_normal_dsr2_input64' folder.
* The dimension of data are as follows
  -- Test_data      =  64x384x1x2304  (channel x scanline x frame x depth)
                        
To perform a test using proposed algorithm

-> Use 'DNN4x1_TestVal' as input data

-> Run 'MAIN_RECONSTRUCTION.m

-> You will get the reconstructed RF data in the 'data\cnn_sparse_view_init_multi_normal_dsr2_input64' directory.

-> Using standard delay-and-sum (DAS) beam-forming code construct a B-mode image. For our experiments we used a DAS beam-forming code provided by (Alpinion Co., Korea). A similar code can be downloaded from ('http://www.ultrasoundtoolbox.com/').

