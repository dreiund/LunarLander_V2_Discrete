# 0. 准备工作
- 利用conda激活一个新的虚拟环境
  
```bash
conda create -n rl_lunar python=3.10 -y
conda activae rl_lunar
```

- 安装系统及依赖（SWIG）用于编译Box2D 物理引擎必须的工具
```bash
conda install -c conda-forge swig
```

- 现在 swig 准备好了，我们用 pip 安装剩下的强化学习库。虽然 Conda 也可以装 Python 包，但 gymnasium 和 stable-baselines3 更新很快，用 pip 能装到最新版且不容易出错。
```bash
pip install "gymnasium[box2d]" stable-baselines3
```

- 安装 TensorBoard 这个工具，用于记录日志&训练曲线
```bash
pip install tensorboard
```

# 1. 实现目标
<img width="625" height="452" alt="截屏2025-12-03 14 17 06" src="https://github.com/user-attachments/assets/dd59450b-07d1-4c2a-ad84-b8d47209e88a" />
