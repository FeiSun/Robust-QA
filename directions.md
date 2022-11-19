## Model Calibrating

### 背景
1. 模型在与训练集分布相似的数据集上效果好，而与训练集分布差别很大的数据集上容易出错。而给出一个错误的答案，比不给答案的危害更大，因此希望模型能够自知、自查。
2. 传统的语言模型都是基于MaxProb来判断答案的correct/incorrect，这种基于probability的方法不可靠


### 目前的研究
1. Percy Liang发表在ACL2020上的一篇paper的做法是：





### Related Words
[Selective Question Answering under Domain Shift](https://aclanthology.org/2020.acl-main.503.pdf)



### 思考
1. 本质问题还是说OOD嘛？为什么要用A模型去测试数据B呢？要是B有足够的数据完全可以送入模型A训练，所以OOD是希望一个模型能够解决所有测试数据嘛？
