# python-a-project
# Alien Invasion
Alien Invasion 是一款基于 Pygame 开发的经典太空射击类游戏，玩家操控飞船射击外星舰队，防止外星人抵达屏幕底部。

## 环境要求
- Python 3.x
- Pygame 库

## 安装步骤
### 1. 安装 Python
前往 [Python 官方网站](https://www.python.org/downloads/) 下载并安装对应系统的 Python 版本（推荐 3.8+），安装时勾选 "Add Python to PATH"。

### 2. 安装 Pygame
打开终端/命令提示符，执行以下命令安装 Pygame：
```bash
pip install pygame
```

## 项目结构
确保代码文件和资源文件的目录结构如下：
```
alien_invasion/
├── images/
│   ├── Ship.jpg       # 飞船图片
│   └── alien.bmp      # 外星人图片
├── alien.py           # 外星人类
├── alien_invasion.py  # 游戏主程序
├── bullet.py          # 子弹类
├── game_stats.py      # 游戏统计信息类
├── settings.py        # 游戏设置类
└── ship.py            # 飞船类
```

## 运行方式
### 1. 克隆/下载代码
将所有代码文件和 `images` 资源文件夹保存到同一目录下。

### 2. 运行主程序
打开终端/命令提示符，切换到代码所在目录，执行以下命令：
```bash
python alien_invasion.py
```

## 游戏操作说明
| 按键 | 功能 |
|------|------|
| ← 方向键 | 向左移动飞船 |
| → 方向键 | 向右移动飞船 |
| 空格键 | 发射子弹 |
| Q 键 | 退出游戏 |

## 游戏规则
1. 游戏启动后，外星舰队会从屏幕右侧向左移动，到达边缘后会向下移动并改变方向；
2. 玩家操控飞船射击外星人，击中后外星人消失；
3. 若外星舰队全部被消灭，会生成新的外星舰队；
4. 若外星人碰撞到飞船或抵达屏幕底部，玩家损失一艘飞船；
5. 玩家初始拥有 3 艘飞船，全部损失后游戏结束。

## 自定义设置（可选）
可修改 `settings.py` 文件调整游戏参数：
- `ship_speed`：飞船移动速度（默认 6）；
- `bullet_speed`：子弹速度（默认 2.0）；
- `alien_speed`：外星人移动速度（默认 1.0）；
- `ship_limit`：玩家初始飞船数量（默认 3）；






- `bullets_allowed`：同时发射的子弹上限（默认 100）；
- `bg_color`：游戏背景色（默认 (230, 230, 230)）。
