# CUDA10.1-and-cdDNN10.1-versionn
測試使用環境架設，基於使用我的環境： Windows 10 CUDA 10.1 Anaconda 3  pytorch ==1.4.0 torchvision == 0.5.0 visdom == 0.1.8.9 OpenCV-Python == 4.5.2.52


### <首先，第一步> 

先了解你的顯卡是多少，找出你下載顯卡的驅動版本。(此部分請看其他網站解釋)
接著！
尋找你所需要的CUDA版本，利用CUDA找出對應的cdDNN。(我們著重的重點)

(ps：當然有時候不一定是CUDA 10.1對應cuDNN 10.1，有可能如下example所示)

(ex：tensorflow_gpu-1.12.0*→*python版本3.5-3.6*→*cdDNN 7.2	*→* CUDA 9.0)

https://www.tensorflow.org/install/source_windows?hl=zh-tw
了解你的tensorflow版本，並找尋所需要的CUDA、cuDNN版本

https://docs.floydhub.com/guides/environments/
了解你的keras與tensorflow所適配之版本，也可看torch

https://pytorch.org/get-started/previous-versions/
了解你的環境與torch所適配之版本


```
已知
我所需要的 pytorch 1.4.0
CUDA 10.1
cdDNN 10.1


```

### <第二步> 
https://developer.nvidia.com/cuda-toolkit-archive
尋找你要的CUDA版本，並下載。

https://developer.nvidia.com/rdp/cudnn-archive
尋找你要的cuDNN版本，並下載。











```
pip install pytorch ==1.4.0
pip install torchvision == 0.5.0
pip install visdom == 0.1.8.9
pip install OpenCV-Python == 4.5.2.52
pip install
```
