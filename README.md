# Alien Invasion 游戏扩展版

一个基于 Pygame 的太空射击游戏，包含多项功能扩展。

## 新增功能

- 最高分持久化保存 - 游戏重启后分数不丢失
- 双难度模式 - 普通模式 vs 困难模式  
- 游戏暂停菜单 - 完整的暂停和恢复功能
- 多难度独立记录 - 每个难度有独立的最高分

## 环境要求

- Python: 3.7 或更高版本
- Pygame: 2.0 或更高版本

## 安装步骤

### 1. 安装 Python
如果还没有安装 Python，请从 Python 官网下载并安装。

### 2. 安装 Pygame
打开命令提示符(Windows)或终端(Mac/Linux)，运行：

```
pip install pygame
```

### 3. 下载游戏代码
```
git clone https://github.com/yourname/alien-invasion
cd alien-invasion
```

或者直接下载 ZIP 文件并解压。

## 运行游戏

进入游戏目录后，运行：

```
python alien_invasion.py
```

## 游戏操作说明

### 开始界面
- 点击 "Play Normal" 开始普通模式游戏
- 点击 "Play Hard" 开始困难模式游戏（敌人速度提升30%）

### 游戏控制
- 左右方向键：移动飞船
- 空格键：发射子弹
- Q键：暂停游戏

### 暂停菜单
游戏暂停时会出现三个选项：
- Resume Game：继续游戏
- Back to Menu：返回开始菜单  
- Exit Game：退出游戏

## 文件说明

- `alien_invasion.py` - 主游戏文件，包含游戏逻辑和暂停功能
- `settings.py` - 游戏设置文件，包含难度配置
- `game_stats.py` - 分数管理，处理最高分保存
- `button.py` - 按钮系统，支持多个按钮显示
- `ship.py` - 玩家飞船控制
- `bullet.py` - 子弹系统
- `alien.py` - 敌人生成和控制
- `images/` - 游戏图片资源文件夹
- `high_scores.json` - 最高分记录文件（自动生成）

## 代码特点

- 完整的注释说明
- 模块化设计
- 错误处理机制
- 可扩展的架构

## 注意事项

- 首次运行会自动创建 high_scores.json 文件
- 不同难度的最高分分别保存
- 游戏退出时会自动保存当前最高分
