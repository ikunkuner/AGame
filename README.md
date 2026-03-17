# Fitness-body-sensor-game

基于Python+MediaPipe的多模块健身体感互动游戏，包含头部躲闪、手脚碰球等健身玩法

## 项目简介

这是一个利用计算机视觉和身体姿态识别技术开发的健身互动游戏项目。通过摄像头捕捉用户的身体动作，使用MediaPipe进行实时姿态检测，实现多种健身游戏模式。该项目旨在将运动与娱乐相结合，提供一种新型的家庭健身方式。

## 主要功能

### 1. 头部躲闪游戏 (pose_realtime.py)
- 使用头部位置控制躲避随机出现的圆圈
- 实时姿态检测和分数统计
- 绿色圆圈随机生成，用户需用头部避开

### 2. 手部控制蛇游戏 (SnakeGame.py)
- 手部跟踪控制蛇的移动
- 吃食物增长长度，避免撞墙
- 实时分数显示和游戏结束判定

### 3. 乒乓球游戏 (Ball.py)
- 双人手部控制挡板
- 球的物理运动模拟
- 分数统计和碰撞检测

### 4. 静态图片姿态检测 (pose_image.py)
- 对静态图片进行人体姿态关键点检测
- 输出关键点坐标信息
- 可用于姿态分析和研究

## 技术栈

- **Python 3.x**
- **MediaPipe**: 人体姿态和手部检测
- **OpenCV**: 图像处理和摄像头操作
- **NumPy**: 数值计算
- **Pygame**: 游戏开发框架
- **Matplotlib**: 数据可视化
- **Pillow**: 图像处理

## 环境要求

- Python 3.7+
- 摄像头设备
- Windows/Linux/macOS

## 安装步骤

1. 克隆项目到本地：
```bash
git clone https://github.com/your-username/Fitness-body-sensor-game.git
cd Fitness-body-sensor-game
```

2. 使用Conda创建虚拟环境：
```bash
# 创建Conda环境（推荐Python 3.8）
conda create -n fitness-game python=3.8
conda activate fitness-game
```

3. 安装依赖包：
```bash
pip install -r requirements.txt
```

## 使用方法

### 运行头部躲闪游戏：
```bash
python pose_realtime.py
```

### 运行蛇游戏：
```bash
python SnakeGame.py
```

### 运行乒乓球游戏：
```bash
python Ball.py
```

### 运行静态图片姿态检测：
```bash
python pose_image.py
```
（需要将图片文件命名为1.jpg放置在项目根目录）

## 项目结构

```
Fitness-body-sensor-game/
├── Ball.py                 # 乒乓球游戏
├── SnakeGame.py           # 蛇游戏
├── pose_realtime.py       # 实时姿态检测游戏
├── pose_image.py          # 静态图片姿态检测
├── requirements.txt       # 项目依赖
├── README.md             # 项目说明
├── LICENSE               # 许可证
└── puck/                 # 游戏资源图片
    ├── ball.png
    ├── block1.png
    ├── block2.png
    ├── desk.png
    └── GG.jpg
```

## 依赖说明

主要依赖包已在requirements.txt中列出：

- opencv-python: 图像处理
- mediapipe: 姿态检测
- numpy: 数值计算
- pygame: 游戏框架
- matplotlib: 可视化
- pillow: 图像处理

## 注意事项

1. 确保摄像头权限已开启
2. 游戏需要良好的光照条件以获得最佳检测效果
3. 建议在空旷环境中进行游戏，避免背景干扰
4. 部分游戏需要手部或全身出现在摄像头视野内

## Conda环境管理

### 退出Conda环境
```bash
conda deactivate
```

### 删除Conda环境
```bash
conda env remove -n fitness-game
```

### 查看所有环境
```bash
conda env list
```

### 为什么使用Conda环境？
- 提供完整的包管理和环境隔离
- 自动解决包依赖冲突
- 支持多种编程语言
- 便于在不同项目间切换环境
- 更好的科学计算包支持（如NumPy, OpenCV等）

## 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 贡献

欢迎提交Issue和Pull Request来改进这个项目！

## 作者

本科毕业设计项目
