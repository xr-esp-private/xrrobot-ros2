# follower — 雷达跟随

## 能力
机器人通过激光雷达识别前方人体，自动跟随移动。

## 启动
```bash
ros2launch xrrobot_follower laser_follower.launch.py
```

## 调用
启动后自动工作。人站在雷达前方，机器人跟随前进。
可通过 RViz2 看到跟随时的人体位置：
```bash
rviz2 -d ~/Desktop/laser_follow.rviz
```

## 依赖
| 需求 | 说明 |
|------|------|
| launch | `laser_follower.launch.py` |
| 前置 | 需要雷达在线 |
| 含 | 底盘（全包） |

## 兼容性
| 可共存 | 说明 |
|--------|------|
| ❌ 其他占用底盘的 | 跟随模式独占底盘控制 |
