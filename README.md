# Compressed-Image-enhancement
[1]AN EFFICIENT DEEP CONVOLUTIONAL NEURAL NETWORKS MODEL FOR COMPRESSED IMAGE DEBLOCKING(ICME 2017)
Ke Li, Bahetiyaer Bare, Bo Yan

1、一个很深的网络结构，每三层有一个跳跃结构
2、ARCNN网络是每一个量化等级训练一个网络，本文则希望一个网络能在不同的量化等级上都得到好的结果，所以训练样本包含不同量化等级的图像
3、adjustable gradient clipping technique
[2] A novel deep learningbased method of improving coding efficiency from the decoder-end for HEVC(DCC 2017)

[3] Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising(TIP 2017)

https://github.com/cszn/DnCNN
[4] Decoder-side HEVC quality enhancement with scalable convolutional neural network (ICME 2017)
42,47  Y-PSNR

https://github.com/ryangBUAA/DS-CNN
[5] ARCNN （ICCV 2015）
第一个做压缩图像（JPEG）增强的深度学习网络，只有四层。

https://github.com/tonitick/AR-CNN
[6] Deep Generative Adversarial Compression Artifact Removal(ICCV 2017)

[7]STD2P: RGBD Semantic Segmentation using Spatio-Temporal Data-Driven Pooling
Yang He1, Wei-Chen Chiu1, Margret Keuper2 and Mario Fritz

https://www.sogou.com/link?url=hedJjaC291MuovqUW6cN1nbJCgvfe_IkFtoJ7Oz0WYE.
[8]Building Dual-Domain Representations for Compression Artifacts Reduction（ECCV 2016）（DDCNN）
Jun Guo, Hongyang Chao

JPEG-compressed
双域学习：DCT and pixel
使用残差学习+Adam加速收敛

[9] A Convolutional Neural Network Approach for Post-Processing in HEVC Intra Coding（VRCNN MMM2017）

22,27,32,37  YUV均测了
2、Multi-Frame Quality Enhancement for Compressed Video （cvpr 2018）
37,42  只增强了Y

[10]Convolutional Neural Network-Based Synthesized View Quality Enhancement for 3D Video Coding（TIP 2018）
Linwei Zhu, Yun Zhang, Shiqi Wang, Hui Yuan, Sam Kwong, Horace H.-S. Ip
      这是一篇将应用到编码框架里面的图，主要影响的是VSO过程，对虚拟视点合成的图像进行增强。直接将压缩后的多个视点作为输入，没有warp过程，然后再进行特征融合增强。
including (30, 39),(35, 42), (40, 45) and (45, 49)

[11] MGANet: A Robust Model for Quality Enhancement of Compressed Video
Xiandong Meng, Xuan Deng, Shuyuan Zhu, Shuaicheng Liu, Chuan Wang, Chen Chen, Bing Zeng
multi-frame guided attention network (MGANet)

60个训练视频  96*96
18个测试视频，JCT-VC class A-E
HM16.9 AI LD  QP=32,37,42 
对比算法：
ARCNN [8], VRCNN [7], MemNet [35], DnCNN [46], DCAD [39] and MFQE [42]

ICIP 2018
1、DEEP RESIDUAL NETWORK FOR ENHANCING QUALITY OF THE DECODED INTRA FRAMES OF HEVC
Fan Li, Weimin Tan, Bo Yan

22, 27, 32, 37, 42 and 47
对比了VRCNN，DSCNN 
指标：BD-rate and BD-PSNR
YUV均增强
2、DMCNN: DUAL-DOMAIN MULTI-SCALE CONVOLUTIONAL NEURAL NETWORK FOR COMPRESSION ARTIFACTS REMOVAL
Xiaoshuai Zhang, Wenhan Yang, Yueyu Hu, Jiaying Liu


JPEG-compressed
双域学习：DCT and pixel
指标：PSNR SSIM PSNR-B
ARCNN、  TNRD、 DnCNN-3、 CAS-CNN、DDCN 
3、ENHANCING HEVC COMPRESSED VIDEOS WITH A PARTITION-MASKED CONVOLUTIONAL NEURAL NETWORK
Xiaoyi He, Qiang Hu, Xiaoyun Zhang, Chongyang Zhang, Weiyao Lin, Xintong Han
       这篇论文主要解决的是增强HEVC压缩后的视频，考虑了coding uint (CU)信息，并将其融合到网络中。提出了一种新的框架，利用分区信息来指导HEVC中基于CNN的质量增强过程，在此框架下，系统地研究了不同的mask generation和mask-frame fusion methods方法，并找到了最佳策略。
QP=22, 27, 32, and 37
 只增强了Y
对比了VRCNN、QECNN-P

AR-CNN [9], DnCNN [46], Li et al. [24]3， DCAD [37] and DS-CNN [42].
