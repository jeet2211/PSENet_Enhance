# PSENet_Enhance
## Description
Progressive Scale Expansion Network (PSENet) is a text detector which is able to well detect the arbitrary-shape text in natural scene

## Dataset
Dataset used: [ICDAR2015](https://rrc.cvc.uab.es/?ch=4&com=tasks#TextLocalization)
A training set of 1000 images containing about 4500 readable words
A testing set containing about 2000 readable words

### [Pretrained Model](#contents)

download pytorch pretrained model: from[Google Drive](https://drive.google.com/file/d/1vIp3sHLmF3xQieIkfDaDSEb8qJMIpoqw/view?usp=drive_link)

## Training
CUDA_VISIBLE_DEVICES=0,1,2,3 python train_ic15.py

## Testing
CUDA_VISIBLE_DEVICES=0 python test_ic15.py --scale 1 --resume [path of model]

## Eval script
cd eval
sh eval_ic15.sh

## results
### [ICDAR 2015](http://rrc.cvc.uab.es/?ch=4&com=evaluation&task=1)
Calculated!{"precision": 0.87, "recall": 0.844, "hmean": 0.857, "AP": 0}
