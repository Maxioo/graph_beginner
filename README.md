# 图神经网络-Beginner
选择一种框架完成如下任务

参考：
- [DGL框架](https://www.dgl.ai/)
- [Pytorch_geometric框架](https://pytorch-geometric.readthedocs.io/en/latest/index.html)
- [子图训练](https://docs.dgl.ai/tutorials/large/L0_neighbor_sampling_overview.html#sphx-glr-tutorials-large-l0-neighbor-sampling-overview-py)

****
## 任务一、 节点分类
实现基于GNN主流模型(GCN, GAT, GraphSAGE, GIN)的节点分类:

1. 实现要求：基于现有模型框架(DGL, Pytorch_geometric)实现图上的节点分类任务
2. 使用Cora, Citeseer, Flickr数据集
3. 测试GCN, GAT, GraphSAGE, GIN模型
4. 利用框架自带的Sampler采样子图进行训练，并与全图训练进行性能和运行时间的对比

## 任务二、 图上的链路预测
1. 实现要求：基于现有模型框架(DGL, Pytorch_geometric)实现图上的链路预测
2. 使用Cora, Citeseer, Flickr数据集
3. 测试GCN, GAT, GraphSAGE, GIN模型
4. 利用框架自带的Sampler采样子图进行训练，并与全图训练进行性能和运行时间的对比

## 任务三、 图分类
1. 实现要求：基于现有模型框架(DGL, Pytorch_geometric)实现图分类任务
2. 使用TUDataset, ZINC数据集
3. 分析不同的池化方法对图分类性能的影响(AvgPooling, MaxPooling, MinPooling)
4. 测试GCN, GAT, GraphSAGE, GIN模型


## 任务四、 知识图谱
1. 参考
   1. 训练和测试框架[KGE框架](https://github.com/Maxioo/kge_framework)
   2. TransE, RotatE, ConvE的论文
2. 实现要求：基于参考资料和知识图谱补全框架，支持常见模型(TransE, RotatE, ConvE)
3. 需要了解的知识点：
   1. 常见知识图谱补全模型的原理(TransE, RotatE, ConvE)
   2. 数据集：训练集/验证集/测试集的划分

## 任务要求
1. 需要了解的知识点：
   1. GNN主流模型的原理(GCN, GAT, GraphSAGE, GIN, ...)
   2. 数据集：训练集/验证集/测试集的划分
2. 代码要求

   代码文件夹按统一格式:
      - 任务一
         - data
         - code
         - README.md
      - 任务二
         - data
         - code
         - README.md
      - ...
      - requirements.txt (运行环境文件)
   
   其中README.md中需要写明训练和测试的脚本

3. 报告要求
   1. 分析不同参数（学习率、网络层数）和不同的神经网络对性能的影响
   2. 测试全图训练和分批次训练对模型性能和运行时间的影响(任务四不需要)