# 补充: 
我没有参考这个环境, 而是直接使用的rlhf哪个环境, 两者很接近, 其实rlhf这个环境也也可命名为`simple_rlhf_trl`
在代码的基础上, 目录中还下载了imdb数据集tokenizer以及gpt2, 总共1.3GB左右
补充.gitignore使用的问题, 不能写成`./model`, 而要写成`/model/`或者`model/`
git缓存问题, 使用`git rm -r --cached .`删除所有缓存, 但慎用, 可以指定某个文件的缓存
# 训练自然语言的LLM模型
包括基于TRL的训练,和手动训练两种实现.

训练方法包括DPO和PPO

环境信息:

python=3.10

torch==2.1.0(cuda)

transformers==4.34.0

datasets==2.14.5

trl==0.7.4

视频课程:https://www.bilibili.com/video/BV1bu4y1w7Dz
