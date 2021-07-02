# CUDA10.1-and-cdDNN10.1-versionn
測試使用環境架設，基於使用我的環境： Windows 10 CUDA 10.1 Anaconda 3  pytorch ==1.4.0 torchvision == 0.5.0 visdom == 0.1.8.9 OpenCV-Python == 4.5.2.52


### <前言> 
先了解你的顯卡是多少，找出你下載顯卡的驅動版本。(此部分請看其他網站解釋)

接著！自己下載anaconda。網址：https://www.anaconda.com/products/individual

尋找你所需要的CUDA版本，利用CUDA找出對應的cdDNN。(我們著重的重點)

(ps：當然有時候不一定是CUDA 10.1對應cuDNN 10.1，有可能如下example所示)

(ex：tensorflow_gpu-1.12.0*→*python版本3.5-3.6*→*cdDNN 7.2	*→* CUDA 9.0)


https://www.tensorflow.org/install/source_windows?hl=zh-tw
了解你的tensorflow版本，並找尋所需要的CUDA、cuDNN版本

https://docs.floydhub.com/guides/environments/
了解你的keras與tensorflow所適配之版本，也可看torch

https://pytorch.org/get-started/previous-versions/
了解你的環境與torch所適配之版本

https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf
conda cheat sheet下載

### <第一步> 
```
已知
我所需要的 pytorch 1.4.0
CUDA 10.1
cdDNN 10.1
```
![image](https://github.com/abcpp12383/CUDA10.1-and-cdDNN10.1-versionn/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-07-02%20155921.png)


https://developer.nvidia.com/cuda-toolkit-archive
尋找你要的CUDA版本，並下載。

https://developer.nvidia.com/rdp/cudnn-archive
尋找你要的cuDNN版本，並下載。
##下載後解壓縮


### <第二步> 創你想要的環境名稱
開啟CMD，再輸入下面的部分

----------------創環境名稱------(方法一)--------------------------

    conda create --name your_env_name python=3.6

注意!!!!your_env_name 是你想要的名稱 我這邊打「torch」

----------------創環境名稱------(方法二)---------((建議使用))-----

    conda create --name your_env_name python=3.6 anaconda

此方法可直接將連結附在Windows 10工具列內 

### <第三步> 在你創的環境名稱下面，安裝你想要的套件
開啟CMD

一、先激活你命名的"torch"環境

    conda activate torch

二、等待出現(torch) C:\Windows\system32

三、在你命名的"torch"環境中，下載torch版本1.4.0 

    conda install pytorch==1.4.0 

四、在你命名的"torch"環境中，下載torchvision版本0.5.0
    
    pip install torchvision==0.5.0 



```
此區是作者安裝的套件部分
conda install pytorch==1.4.0
conda install torchvision==0.5.0
pip install visdom==0.1.8.9
pip install OpenCV-Python==4.5.2.52
pip install pip install matplotlib
pip install jupyter notebook
```
----------------------附記-----------------------------------

#ModuleNotFoundError: No module named ‘cv2’

在安裝 opencv 時會出現 ImportError: No module named cv2 的錯誤，找不到 cv2 的包。

這時候安裝擴充套件包即可：

    pip install opencv-python
----------------------附記-----------------------------------

想要使用jupyter 請一定要自己安裝擴充套件包即可:

    pip install jupyter notebook

其他必要的

    pip install matplotlib
