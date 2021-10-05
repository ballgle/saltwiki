用阿里云加速cuda安装ubuntu20.04)

```
wget https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/cuda-ubuntu2004.pin
sudo mv cuda-ubuntu2004.pin /etc/apt/preferences.d/cuda-repository-pin-600
sudo apt-key adv --fetch-keys https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/7fa2af80.pub
sudo add-apt-repository "deb https://mirrors.aliyun.com/nvidia-cuda/ubuntu2004/x86_64/ /"
sudo apt-get update
sudo apt-get -y install cuda-11-1
```
