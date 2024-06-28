
https://github.com/NVlabs/stylegan2-ada-pytorch

<br>

$ nvidia-smi

https://developer.nvidia.com/cuda-12-2-0-download-archive?target_os=Linux&target_arch=x86_64&Distribution=Ubuntu&target_version=22.04&target_type=deb_local

https://pytorch.org/

https://velog.io/@dongju101/error-externally-managed-environment-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0

 -> sudo rm /usr/lib/python3.11/EXTERNALLY-MANAGED

https://github.com/NVlabs/stylegan2-ada-pytorch

pip install setuptools

sudo apt install nvidia-cuda-toolkit

<br><br>

https://github.com/yuval-alaluf/SAM

<br>

pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121

pip install ninja setuptools matplotlib tqdm

python scripts/inference_side_by_side.py \
--exp_dir=results/output \
--checkpoint_path=results/sam_ffhq_aging.pt \
--data_path=results/input \
--test_batch_size=4 \
--test_workers=4 \
--target_age=0,10,20,30,40,50,60,70,80


<br><br><br><br>

sudo apt install python3-venv

python3 -m venv 'venvname'

source 가상 환경 경로/bin/activate


<br><br><br>

<p float="left">
 <img src = "files/1.jpeg" width="30%" height="30%">
 <img src = "files/1_downscaled.jpg" width="30%" height="30%">
 <img src = "files/1_upscaled.png" width="30%" height="30%">
</p>
