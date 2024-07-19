
Ubuntu 에서 테스트하였음 

https://docs.anaconda.com/anaconda/install/linux/ 에서 Anaconda설치

https://github.com/hafriedlander/SmallDogBig 에서 파일을 받은 후 

```
conda env create -f environment.yaml
conda activate smalldogbig
```

Weights 문단에 있는 `.pt`파일 다운로드 

`python smalldogbig.py` 실행


<br><br><br>
https://github.com/NVlabs/stylegan2-ada-pytorch

`$ nvidia-smi 에서` 
`Driver Version`과 `CUDA Version` 확인 후 

`https://pytorch.org/` 에서 알맞는 버전 선택(12.1 작동 확인함) 후 설치

홈페이지에서 제공하는 명령 : `pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121`

기타 필요한 의존성 파일 설치 시 `error: externally-managed-environment` 에러가 발생하면 

`sudo rm /usr/lib/python3.11/EXTERNALLY-MANAGED` 로 해결


<br><br><br>
pip install setuptools

sudo apt install nvidia-cuda-toolkit



<br><br><br>

https://github.com/yuval-alaluf/SAM

<br>

```
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121

pip install ninja setuptools matplotlib tqdm

python scripts/inference_side_by_side.py \
--exp_dir=results/output \
--checkpoint_path=results/sam_ffhq_aging.pt \
--data_path=results/input \
--test_batch_size=4 \
--test_workers=4 \
--target_age=0,10,20,30,40,50,60,70,80
```

<br><br><br><br>

```
sudo apt install python3-venv

python3 -m venv 'venvname'

source 가상 환경 경로/bin/activate
```


```
libstdc++.so.6: version `glibcxx_3.4.30' not found


// 해당 버전을 포함하고 있는 gcc compiler 버전을 설치해주어 해결했다. 환경 분석이 생각보다 오래걸리니 참고하자.

$ conda install -c conda-forge gcc=12.1.0

glibcxx_3.4.30 가 없어서 gcc 12.1.0 을 설치해줬지만, 추후에 비슷한 문제가 발생한다면 해당하는 gcc 버전을 찾아서 설치해주면 될 것 같다. 


conda install -c conda-forge gxx_linux-64
```

```
ImportError: /home/nxrlab/miniconda3/envs/eg3d/lib/python3.9/site-packages/../../libstdc++.so.6: version `GLIBCXX_3.4.32' not found (required by /home/nxrlab/.cache/torch_extensions/py39_cu111/bias_act_plugin/b46266ff65f9fa53c32108953a1c6f16-nvidia-geforce-rtx-3080/bias_act_plugin.so)

nxrlab@nxrlab:~/Downloads/eg3d$ conda install -c conda-forge libstdcxx-ng
```
