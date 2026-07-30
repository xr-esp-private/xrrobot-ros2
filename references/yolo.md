# yolo — YOLO 数据采集与训练

## 能力
在机器人端进行 YOLO 目标检测数据采集、标注、训练、部署一条龙。

## 启动
```bash
ros2launch xrrobot_yolo_studio xrrobot_yolo_studio.launch.py
```

## 调用
Web 界面操作：浏览器访问 `http://<机器人IP>:8091`
- 选择/创建数据集
- 冻结画面画框标注
- 训练模型（或导出到电脑训练）
- 部署模型并测试

## 依赖
| 需求 | 说明 |
|------|------|
| launch | `xrrobot_yolo_studio.launch.py` |
| 前置 | 无（不依赖底盘/相机/雷达，独立运行） |

## 兼容性
| 可共存 | 说明 |
|--------|------|
| ✅ navigation | 导航中也可以做目标检测 |
| ✅ camera | 共用摄像头 |
| ✅ grasp | 视觉抓取可调用 YOLO 模型 |
| ✅ 任何其他 | 完全独立，不冲突 |
