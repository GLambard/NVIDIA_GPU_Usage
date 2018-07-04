# NVIDIA GPU usage in the blink of an eye :zap: :smiley:

Use of [nvidia-smi](https://developer.nvidia.com/nvidia-system-management-interface) 

## How
In a teminal, type
```
nvidia-smi -l 2
```
which results in something like this re-newed each 2 seconds
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
