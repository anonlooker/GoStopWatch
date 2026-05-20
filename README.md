# GoStopWatch

[中文](README.zh-cn.md)

A simple stopwatch GUI application built with Go and [Fyne](https://fyne.io/).

## Screenshot

```
+----------------------------------+
|           Stopwatch              |
|                                  |
|         00:01:23.45              |
|                                  |
|    [ Start ] [ Stop ] [ Reset ]  |
+----------------------------------+
```

## Features

- **Start** — begin or resume the stopwatch
- **Stop** — pause and accumulate elapsed time
- **Reset** — stop and zero the clock
- Display format: `HH:MM:SS.ms`
- Thread-safe timing with mutex locks
- 10 ms tick precision

## Prerequisites

- Go 1.25+
- X11 development libraries (Linux)

```bash
sudo apt-get install -y libgl1-mesa-dev libxxf86vm-dev libx11-dev libxrandr-dev libxi-dev libxcursor-dev libxinerama-dev
```

## Build & Run

```bash
go build -o stopwatch .
./stopwatch
```

Or run directly:

```bash
go run .
```

## License

[MPL-2.0](LICENSE)
