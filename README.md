RHCell(Radiation-Hardened Cell)

# ENV Init
```shell
conda create --name RH python=3.9 -y
conda activate RH
```
# PLACE Package

有GPU 
```shell
pip install torch==2.5.1+cu121 torchvision==0.20.1+cu121 torchaudio==2.5.1     --index-url https://download.pytorch.org/whl/cu121
pip install torch_geometric==2.6.1 -f https://data.pyg.org/whl/torch-2.5.1+cu121.html
```
无GPU 
```shell
pip install torch==2.5.1 torchvision==0.20.1 torchaudio==2.5.1
pip install torch_geometric==2.6.1 -f https://data.pyg.org/whl/torch-2.5.1.html
```
通用
```shell
pip install stable-baselines3[extra]==2.6.0 gymnasium==0.29.1
pip install notebook jupyterlab
```
# Route Package
```shell
pip install scipy
pip install mplcursors
pip install gdspy
```

gdspy 在windows 需额外安装C++拓展模块。若命令报错，建议咨询AI或在linux中使用或暂时放弃输出GDS，注释相关代码
