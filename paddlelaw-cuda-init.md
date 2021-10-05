用阿里云加速cuda安装ubuntu20.04)

```
wget https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/cuda-ubuntu2004.pin
sudo mv cuda-ubuntu2004.pin /etc/apt/preferences.d/cuda-repository-pin-600
sudo apt-key adv --fetch-keys https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/7fa2af80.pub
sudo add-apt-repository "deb https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/ /"
sudo apt-get update
sudo apt-get -y install cuda-11-1
```

官方安装指南

···

conda install -c rapidsai -c nvidia -c numba -c conda-forge cudf=21.06 python=3.7 cudatoolkit=11.4

wget https://developer.download.nvidia.com/compute/cuda/repos/wsl-ubuntu/x86_64/cuda-wsl-ubuntu.pin
sudo mv cuda-wsl-ubuntu.pin /etc/apt/preferences.d/cuda-repository-pin-600
wget https://developer.download.nvidia.com/compute/cuda/11.4.2/local_installers/cuda-repo-wsl-ubuntu-11-4-local_11.4.2-1_amd64.deb
sudo dpkg -i cuda-repo-wsl-ubuntu-11-4-local_11.4.2-1_amd64.deb
sudo apt-key add /var/cuda-repo-wsl-ubuntu-11-4-local/7fa2af80.pub
sudo apt-get update
sudo apt-get -y install cuda


$ wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/cuda-ubuntu2004.pin
$ sudo mv cuda-ubuntu2004.pin /etc/apt/preferences.d/cuda-repository-pin-600
$ wget https://developer.download.nvidia.com/compute/cuda/11.4.0/local_installers/cuda-repo-ubuntu2004-11-4-local_11.4.0-470.42.01-1_amd64.deb
$ wget https://developer.download.nvidia.com/compute/cuda/11.4.2/local_installers/cuda-repo-ubuntu2004-11-4-local_11.4.2-470.42.01-1_amd64.deb
$ sudo dpkg -i cuda-repo-ubuntu2004-11-4-local_11.4.0-470.42.01-1_amd64.deb
$ sudo apt-key add /var/cuda-repo-ubuntu2004-11-4-local/7fa2af80.pub
$ sudo apt-get update

https://blog.csdn.net/momodosky/article/details/119673472  总体 

https://zhuanlan.zhihu.com/p/356397851  升级wsl1为wsl2

https://zhuanlan.zhihu.com/p/350399229  win10的wsl2安装cuda并配置pytorch]

https://blog.csdn.net/Veritaz/article/details/113826386 用阿里云镜像加速CUDA安装（Ubuntu20.04）

wget https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/cuda-ubuntu2004.pin
sudo mv cuda-ubuntu2004.pin /etc/apt/preferences.d/cuda-repository-pin-600
sudo apt-key adv --fetch-keys https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/7fa2af80.pub
sudo add-apt-repository "deb https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/ /"
sudo apt-get update
sudo apt-get -y install cuda-11-1

···
