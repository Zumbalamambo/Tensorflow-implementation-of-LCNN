#  Light CNN for Deep Face Recognition, in Tensorflow
A Tensorflow implementation of [A Light CNN for Deep Face Representation with Noisy Labels](https://arxiv.org/abs/1511.02683) from the paper by Xiang Wu 

## Updates
- Sep 20, 2017
	- Add model and evaluted code.
	- Add training code.
- Sep 19, 2017
	- The repository was built.


## Datasets
- Training data
	- Download face dataset [MS-Celeb-1M (Aligned)](http://www.msceleb.org/download/aligned).
	- All face images are RGB images and resize to **122x144** 
- Testing data
	- Download aligned LFW (122*144) [images](https://1drv.ms/u/s!AleP5K29t5x7ge88rngfpitnvpkZbw) and [list](https://1drv.ms/t/s!AleP5K29t5x7ge9DV6jfHo392ONwCA)

## Training 
- Add

## Evaluation
- Download [LCNN-29 model](https://1drv.ms/f/s!AleP5K29t5x7ge89GqB3Ue_Pe5rN3A)
- Download [LFW features](https://1drv.ms/u/s!AleP5K29t5x7ge9ElofW_tDzxCq5sw)

## Performance
The Light CNN performance on lfw 6,000 pairs.   

|   Model | traing data	| method |100% - EER | TPR@FAR=1%   | TPR@FAR=0.1%| TPR@FAR=0| 
| :------- | :----: | :----: | :----: | :---: | :---: |:---: | 
| LightCNN-29 (Wu Xiang)| 70K/-	|Softmax|99.40% | 99.43% | 98.67% | 95.70% |
| LightCNN-29 (Tensorflow)|10K/- |Softmax|98.2% |    97.73%    |    92.26%  |    60.53%  | 
| LightCNN-29 (Tensorflow)|10K/- |Softmax+L2|98.26% |    97.76%    |    95%  |    55.9%  | 
| LightCNN-29 (Tensorflow)|10K/- |Softmax+L2+PCA|98.43% |    98.1%    |    94.26%  |    73.26%  | 
| LightCNN-29 (Tensorflow)|10K/- |Softmax+L2+PCA|98.5% |    98.2%    |    96.06%  |    81.83%  |


## Referencs
- [Original Light CNN implementation (caffe)](https://github.com/AlfredXiangWu/face_verification_experiment).
