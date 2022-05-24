# HGATE: Heterogeneous Graph Attention Auto-Encoders

# Paper
HGATE: Heterogeneous Graph Attention Auto-Encoders

Graph auto-encoder is considered a framework for unsupervised learning on graph-structured data by representing graphs in a low dimensional space. It has been proved very powerful for graph analytics. In the real world, complex relationships in various entities can be represented by heterogeneous graphs that contain more abundant semantic information than homogeneous graphs. In general, graph auto-encoders based on homogeneous graphs are not applicable to heterogeneous graphs. In addition, little work has been done to evaluate the effect of different semantics on node embedding in heterogeneous graphs for unsupervised graph representation learning. In this work, we propose a novel Heterogeneous Graph Attention Auto-Encoders (HGATE) for unsupervised representation learning on heterogeneous graph-structured data. Based on the consideration of semantic information, our architecture of HGATE reconstructs not only the edges of the heterogeneous graph but also node attributes, through stacked encoder/decoder layers. Hierarchical attention is used to learn the relevance between a node and its meta-path based neighbors, and the relevance among different meta-paths.HGATE is applicable to transductive learning as well as inductive learning. Node classification and link prediction experiments on real-world heterogeneous graph datasets demonstrate the effectiveness of HGATE for both transductive and inductive tasks.

# Citation
```
@ARTICLE{9664297,
  author={Wang, Wei and Wei, Xiangyu and Suo, Xiaoyang and Wang, Bin and Wang, Hao and Dai, Hong-Ning and Zhang, Xiangliang},
  journal={IEEE Transactions on Knowledge and Data Engineering}, 
  title={HGATE: Heterogeneous Graph Attention Auto-Encoders}, 
  year={2021},
  volume={},
  number={},
  pages={1-1},
  doi={10.1109/TKDE.2021.3138788}
 }
 ```

## Requirements
* tensorflow (1.14)
* sklearn
* pandas
* numpy

## Run the demo

# inductive learning
```bash
python3 inductive_weibo.py
```

# transductive learning
```bash
python3 transductive_weibo.py
```


## Data

In order to use your own data, you have to provide
* an N by N adjacency matrix, where N is the number of nodes;
* an N by F node attribute feature matrix, where F is the number of attributes features per node;
* an N by E binary label matrix, where E is the number of classes.

