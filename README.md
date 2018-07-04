# NVIDIA GPU usage monitoring in the blink of an eye :zap: :smiley:

Use of [nvidia-smi](https://developer.nvidia.com/nvidia-system-management-interface) 

## System OS

- Linux (Ubuntu, CentOS, ...) 
- 64-bit Windows Server 2008 R2 
- Windows 7

- For MacOSX, please check ```cuda-smi``` command from [here](https://github.com/phvu/cuda-smi)

## How
In a teminal, type
```
nvidia-smi -l 2
```
or with the ```watch ``` command for not fullfilling your terminal 
(through Cygwin for Windows, or installable through homebrew/macports on MacOSX), 

```
watch -d -n 2 nvidia-smi *(cuda-smi for MacOSX)*
```

which results in monitoring your GPU(s) usage re-newed each 2 seconds
```
+-----------------------------------------------------------------------------+
| NVIDIA-SMI 387.34                 Driver Version: 387.34                    |
|-------------------------------+----------------------+----------------------+
| GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
|===============================+======================+======================|
|   0  Graphics Device     Off  | 00000000:01:00.0 Off |                  N/A |
| 37%   53C    P2    46W / 250W |  11794MiB / 12058MiB |     70%      Default |
+-------------------------------+----------------------+----------------------+
                                                                               
+-----------------------------------------------------------------------------+
| Processes:                                                       GPU Memory |
|  GPU       PID   Type   Process name                             Usage      |
|=============================================================================|
|    0      1606      G   /usr/lib/xorg/Xorg                           415MiB |
|    0      4315      G   compiz                                       186MiB |
|    0     19879      G   ...-token=<hash>                             142MiB |
|    0     28315      C   ...<user>/miniconda3/envs/py36/bin/python  11036MiB |
+-----------------------------------------------------------------------------+
```

# Hope it helps! :smiley:
