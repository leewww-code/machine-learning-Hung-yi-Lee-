涉及数据增强相关知识，后面再更新
大体思路  

1. 0.05验证集和训练集的切分(增加训练数据 百万级的数据集正常划分标准)

2. batch size 1024 加速coding的进程；batch size和learning rate需要同步调整
3. epoch 设置为100；learing rate=1e-5;weight_decay=1e-4
64 128 256 512 1024
4. 
scheduler = torch.optim.lr_scheduler.CosineAnnealingWarmRestarts(optimizer,T_0=10,verbose=False)
5. 
 预测上下文之间存在某种规律
6. “简单的”DNN: 8 2？ Layers+数据处理
7. 不均衡的数据集
from torch.utils.data import WeightedRandomSampler

