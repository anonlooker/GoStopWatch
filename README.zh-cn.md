# GoStopWatch

[English](README.md)

使用 Go 和 [Fyne](https://fyne.io/) 构建的简易秒表 GUI 应用。

## 界面

```
+----------------------------------+
|           秒表                   |
|                                  |
|         00:01:23.45              |
|                                  |
|    [ 开始 ] [ 停止 ] [ 重置 ]    |
+----------------------------------+
```

## 功能

- **开始** — 启动或继续计时
- **停止** — 暂停并累计已用时间
- **重置** — 停止计时并归零
- 显示格式：`HH:MM:SS.ms`
- 使用互斥锁保证线程安全
- 10 毫秒刷新精度

## 环境要求

- Go 1.25+
- X11 开发库（Linux）

```bash
sudo apt-get install -y libgl1-mesa-dev libxxf86vm-dev libx11-dev libxrandr-dev libxi-dev libxcursor-dev libxinerama-dev
```

## 构建与运行

```bash
go build -o stopwatch .
./stopwatch
```

或直接运行：

```bash
go run .
```

## 许可证

[MPL-2.0](LICENSE)
