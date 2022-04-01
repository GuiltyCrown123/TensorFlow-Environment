# TensorFlow-Environment

**建議一開始使用Geforce Experience將GPU驅動更新**

Step1. Install Anaconda (安裝過程記得加入環境變數中)

Conda語法:
conda -V #conda --version

1. Conda list

2. conda update pip  (保留未必要打)

3. conda install lxml


[在 conda 下裝 tensorflow-gpu 2.0/2.1/2.6 ] 
--------------------------------------------------------------------
使用 conda 安裝 tensorflow 2.0/2.1 會自動安裝 cuda10.0, cudnn7.6, 不用在 window 安裝 cuda10
              tensorflwo 2.6                          cudnn8.2

Ref:  https://www.youtube.com/watch?v=qLjw_EtqmCs

查 codna tensorflow-gpu 可用版: conda search tensorflow-gpu

查 tensorflow-gpu 安裝匹配 ref: https://tensorflow.google.cn/install/source_windows?hl=cn#gpu%20%E4%BD%9C%E8%80%85%EF%BC%9Atm9161%20https://www.bilibili.com/read/cv9003982%20%E5%87%BA%E5%A4%84%EF%BC%9Abilibili

[tf2.1]
1. conda create --name tf2.1 python=3.7 [ok]
2. conda activate tf2.1
3. conda install tensorflow-gpu=2.1
   conda install keras
4. conda install matplotlib
5. conda install nb_conda [需 python 3.8 以下]
   jupyter notebook
6. conda install spyder
   spyder
   
 [Condition Solution]
 TensorFlow 在執行时，在Adding visible gpu devices: 0卡很久:
 1. 至環境變數-系統變數,加入【CUDA_CACHE_MAXSIZE=4294967296】
 
 2. 確認完成，並重新開機




