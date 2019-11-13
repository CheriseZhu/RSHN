# RSHN
The implementation of our ICDM 2019 paper "Relation Structure-Aware Heterogeneous Graph Neural Network" RSHN.

# Requirements
python == 3.6.2<br>
torch == 1.1.0<br>
numpy == 1.16.4<br>
scipy == 1.2.0<br>
torch_geometric == 1.0.0<br>
numba == 0.42.1

# How to use
  ### Dataset
  The data folder includes our propocessed data for training and testing. <br>
  The orginal datasets can be founded from [here](https://s3.us-east-2.amazonaws.com/dgl.ai/dataset).

  ### Model
  The model folder includes our proposed model "RSHN".<br>
  The build_coarsened_line_graph folder includes utils used in model.<br>
  The torch_geometeric/nn/conv folder includes the designed convolution layers used in model. 
  
  ### Training/Testing
  ```
  cd model
  python RSHN.py --dataset AIFB --lr 0.01 --weight_decay 5e-4 --dim 16 --num_node_layer 2 --num_edge_layer 1 --dropout 0.6 --epoch 50
  ```
  
  
# Citation
```
@inproceedings{zhu2019RSHN
author={Shichao Zhu and Chuan Zhou and Shirui Pan and Xingquan Zhu and Bin Wang},
title={Relation Structure-Aware Heterogeneous Graph Neural Network},
journal={IEEE International Conference On Data Mining (ICDM)},
year={2019}
}
```
