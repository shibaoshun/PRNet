# PRNet
# Abstract
Recovering the image of interest from its phaseless measurement is the goal of phase retrieval (PR). Recent PR algorithms that use hand-crafted priors suffer from low-quality reconstructions in the case of high noise levels. To cope with this limitation, we propose a novel deep unfolded phase retrieval network dubbed as PRNet to recover high-quality images by using the learned convolutional sparse coding (CSC). Concretely, we formulate a convolutional sparse coding phase retrieval optimization problem, and solve it by using an iteration optimization algorithm consisting two steps, i.e., the CSC and image updating steps. We unroll the proposed iteration algorithm to construct a deep network, and involve an adaptive thresholding network (ATN) to enhance the represent ability of the learned CSC. The ATN can exploit relationship of channels to determine the thresholds for CSC. Experiments demonstrate that the proposed PRNet can recover high-quality images at high noise levels.

# Requirement
Python 3.7.4\
PyTorch 1.7.0+cu110\
torchvision 0.4.1\
numpy 1.19.5
## How to obtain the trained models
The trained models can be found at:  https://pan.baidu.com/s/1a0eDW-gnN1aIkTts29k6WA, the pass word of the file is `fr6l`.
# Testing
The files of PRNet_~dB contain the trained models and the parameters of the ADAM optimizer at different noise levels.\
Test_SNR.py is utilize to test the PSNR and SSIM values of the proposed PRNet on Set12.\
By modifying the the name of model and the value of SNR in Test_SNR.py, evaluating the imaging quality of the proposed PRNet at different SNRs can be achieved.\
If you encounter any problems, please do not hesitate to contact me.
E-mail: shibaoshun@ysu.edu.cn
