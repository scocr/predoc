#### OCR算法简介（https://www.zhihu.com/question/20191727）
#####  步骤：
	1. decection  找到包含文字的区域proposal
	# 可以利用radon hough等变换进行文本校正
	2. classification 识别区域中的文字
	3. 基于统计模型进行语义纠错(N-gram,CRF等)

#####  水平文字检测  
	CTPN  Connectionist Text Proposal Network 从Faster R-CNN改进而来
		文章：https://zhuanlan.zhihu.com/p/34757009
		Paper：https://arxiv.org/abs/1609.03605
	Faster R-CNN文章：https://zhuanlan.zhihu.com/p/31426458（详读与实现）

#####  倾斜文字检测  
	EAST An Efficient and Accurate Scene Text Detector
		文章：https://zhuanlan.zhihu.com/p/37504120
		Paper：https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/1704.03155.pdf
	SegLink  Detecting Oriented Text in Natural Images by Linking Segments 
		文章：https://zhuanlan.zhihu.com/p/37781277
		地址：https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/1703.06520.pdf
	

#####  文字识别算法
	CRNN（CNN+RNN+CTC）算法  
		文章：https://zhuanlan.zhihu.com/p/43534801
		Paper：https://arxiv.org/abs/1507.05717

	CNN+Seq2Seq+Attention
		文章：https://zhuanlan.zhihu.com/p/51383402
	

##### end-to-end 文字检测与识别(主要是针对水平文字检测)
	Towards End-to-end Text Spotting with Convolutional Recurrent Neural Networks



##### Git模型实例
	文本检测与识别模型： CTPN + DenseNet + CTC
	https://github.com/YCG09/chinese_ocr
	
	文本检测模型：Connectionist Text Proposal Network
	https://github.com/eragonruan/text-detection-ctpn

	文本检测模型： Shape Robust Text Detection with Progressive Scale Expansion Network   
	GIT第地址： 
	pytorch   https://github.com/whai362/PSENet
	tensorflow   https://github.com/liuheng92/tensorflow_PSENet

	倾斜文本检测模型： EAST
	tensorflow    https://github.com/argman/EAST
	倾斜文本检测模型： SegLink
	tensorflow    https://github.com/bgshih/seglink
	

	文字识别模型：CRNN（CNN + RNN） + CTC
	https://github.com/bai-shang/OCR_TF_CRNN_CTC

##### 训练数据集：
	查看 https://github.com/liuheng92/tensorflow_PSENet  下的Download模块
	http://www.robots.ox.ac.uk/~vgg/data/text/
