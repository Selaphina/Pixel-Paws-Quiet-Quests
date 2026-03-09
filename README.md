# Pixel Paws Quiet Quests 🐕

> 一款像素风格的解谜小游戏，控制小狗寻找并关闭噪音源，让小屋重归宁静。补档2023年7月的arduino+processing开发大作业。

## 🎮 游戏运行截图


鼠标控制小狗在房间内移动，点击家具物品进行互动，找到并关闭收音机 (外接arduino蜂鸣器)，停止噪音。

## 📁 项目结构

```
├── pixelGame/
│   ├── pixelGame.pde    # 主游戏代码 (Processing)
│   └── data/            # 游戏素材（像素图片、音效）
├── arduinoProject/
│   └── akanong_*.ino    # Arduino音乐控制程序
└── README.md
```

## 🛠️ 技术栈

- **交互逻辑**：Processing
- **硬件控制**: Arduino (可选，用于播放音乐)

## 🚀 运行方式

### 运行游戏

1. 下载并安装 [Processing](https://processing.org/)
2. 打开 `pixelGame/pixelGame.pde`
3. 点击运行按钮 ▶️

### (可选) Arduino 音乐模块

1. 将 Arduino 连接到扬声器（引脚 6）
2. 通过串口（COM9, 9600波特率）与游戏通信
3. 游戏可通过串口控制播放/停止音乐

## 📝 开发小记

- 游戏采用多页面架构：主菜单 → 游戏关卡 → 成功 → 通关动画
- 支持与多种物品交互：咖啡机、饮料柜、冰箱、打印机等
- 鼠标悬停高亮提示可交互物品

