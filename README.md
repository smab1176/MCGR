# MCGR
## Remote Sensing Image Super-resolution and Object Detection: Benchmark and State of the Art
Yi Wang, Syed Muhammad Arsalan Bashir, Mahrukh Khan, Qudrat Ullah, Rui Wang, Yilin Song, Zhe Guo, and Yilong Niu 

Northwestern Polytechnical University

The overall framework of the proposed method is shown below where RFA-based generator is used in a Wasserstein GAN has with a weighted loss function for multi-class object detection using image SR.
![Fig  1](https://github.com/smab1176/MCGR/blob/90bd113669b2aa7e97cfcd45cff183d0dae46fe6/Figure%202-7.png)

Image SR performance comparison in terms of MSE, PSNR and SSIM on the propsoed RSSOD dataset (https://data.mendeley.com/datasets/b268jv86tf/1) is shown in Table 1.

**Table 1.** Performance comparison for a scale factor of 4 (Bold = best results, bold-italic = second-best).

Method          | MSE       | PSNR (dB) | SSIM
----------------|-----------|-----------|----------
Bicubic 	      |  79.99	  |  30.23	  |   0.79
Real-ESRGAN 	  |  72.54	  |  30.81	  |   0.81
SwinIR-L 	      |  65.34	  |  30.90	  |   0.76
BSRGAN 	        |  58.26	  |  31.85	  |   0.82
DRN	            |  44.89	  |  32.69	  |   0.85
EDSR	          |  37.64	  |  33.13	  |   ***0.89***
NLSN	          |  ***31.17***	  |  ***33.48***	  |   0.88
MCGR	          |  **27.98**	|  **34.68**	  |   **0.93**




Detection performance in-terms of  Impact of change in detector network on mAP for an IoU is shown in Table 2. 

**Table 2.** The impact of scale factor on the detection mAP with an IoU of 0.10 on a five-class test set (Bold = best results, bold-italic = second-best).

Method           | HR(mAP)    | mAP@SF=2 | mAP@SF=4 |  Inference time (ms)
-----------------|-------|---------|----------|-----------------
YOLOv5	         |**0.76** | ***0.68***|	***0.58***	  |  **4.33**
RetinaNet	       |  0.50 |   0.44	 |  0.21	  |    93.64
SSD (VGG16)	     |  0.51 |   0.43	 |  0.27	  |    31.10
Faster R-CNN	   |  0.68 |   0.53	 |  0.44	  |    88.14
EfficientDet-D5	 |  0.72 |   0.57	 |  0.46	  |    52.31
MCGR	           | ***0.75***|**0.731**|	**0.71**  |   ***16.61***


**Paper Reference**

Yi Wang, Syed Muhammad Arsalan Bashir, Mahrukh Khan, Qudrat Ullah, Rui Wang, Yilin Song, Zhe Guo, Yilong Niu (2021). Remote Sensing Image Super-resolution and Object Detection: Benchmark and State of the Art. **arXiv**, https://arxiv.org/abs/2111.03260


For queries contact:
**smarsalan(at)mail(dot)nwpu(dot)edu(dot)cn**
