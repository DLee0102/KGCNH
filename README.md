# Requirments
Pytorch==2.0.1

dgl==1.1.2

scikit-learn==1.3.0

python==3.9.18

# How to use
if your cuda is available, you can 
run python ./code/main.py --gpu --enable_augmentation --enable_gumbel

else 
run python ./code/main.py --enable_augmentation --enable_gumbel

# （DL）安装注意事项
1. 在dgl官方网站找到安装文档后修改安装语句为如下，否则会报各种dll错误，cuda不匹配等（我的环境为cuda11.7）：
```python
pip install  dgl==1.1.2 -f https://data.dgl.ai/wheels/cu117/repo.html
```