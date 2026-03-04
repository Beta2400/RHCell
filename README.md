RHCell(Radiation-Hardened Cell)

# ENV init
conda create --name RH python=3.9 -y

conda activate RH

# place init
有GPU pip install torch==2.5.1+cu121 torchvision==0.20.1+cu121 torchaudio==2.5.1     --index-url https://download.pytorch.org/whl/cu121

无GPU pip install torch==2.5.1 torchvision==0.20.1 torchaudio==2.5.1 

pip install stable-baselines3[extra]==2.6.0 gymnasium==0.29.1

有GPU pip install torch_geometric==2.6.1 -f https://data.pyg.org/whl/torch-2.5.1+cu121.html

无GPU pip install torch_geometric==2.6.1 -f https://data.pyg.org/whl/torch-2.5.1.html

pip install notebook jupyterlab

# For Route
pip install scipy

pip install mplcursors

window 需安装C++拓展模块。若命令报错，建议咨询AI，在linux中使用或暂时放弃输出GDS

pip install gdspy
