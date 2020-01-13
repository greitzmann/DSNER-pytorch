# DNSER-pytorch
Pytorch implementation of  :https://github.com/rainarch/DSNER

python 3.6

pytorch

First: python script/preprocess-EC

main module: python dsner.py

args parameters should be define based on the paper

Result: Dev and Test respectively

|	Model      |	Setup  |   epoch   |   P   |   R   |   F1  |  P    | R     | F1    |
|--------------|-----------|-----------|-------|-------|-------|-------|-------|-------|
|LSTM+CRF      |	H      |	562    |66.30 %|64.21 %|65.24 %|63.64 %|62.53 %|63.08 %|
|LSTM+CRF      |  H+A	   |    769    |67.80 %|58.53 %|62.82 %|63.65 %|53.59 %|58.19 %|
|LSTm+CRF+SL   |  H+A      |	538    |68.21 %|61.89 %|64.90 %|66.90 %|61.66 %|64.17 %|
|LSTm+CRF+PA   |  H+A      |	652    |62.21 %|70.11 %|65.93 %|61.12 %|67.63 %|64.21 %|
|LSTm+CRF+PA+SL|H+A	       |    370    |69.12 %|71.16 %|70.12 %|63.46 %|63.94 %|63.70 %|

Another paper which is used RL as post-Processing for denoising with different reward formula:
Reinforcement-based denoising of distantly supervised NER with partial annotation : https://www.aclweb.org/anthology/D19-6125/
