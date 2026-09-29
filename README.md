# RobotMasterHello

一个简单的 C++ 控制台程序，运行后输出 `Hello, RobotMaster!`。

## 环境要求

- Windows 10 或更高版本
- CMake 3.10 或更高版本
- 已安装并配置好的 C++ 编译器，例如 Visual Studio、MinGW-w64 或 Clang

## 构建与运行

在项目根目录打开 PowerShell，执行：

```powershell
cmake -S . -B build
cmake --build build --config Release
```

Visual Studio 等多配置生成器的运行命令：

```powershell
.\build\Release\RobotMasterHello.exe
```

MinGW、Ninja 等单配置生成器通常使用：

```powershell
.\build\RobotMasterHello.exe
```

## 预期输出

```text
Hello, RobotMaster!
```

## 目录结构

```text
作业一/
├── CMakeLists.txt       # CMake 构建配置
├── main.cpp             # 程序入口
├── README.md            # 项目说明
├── CMakelist.txt        # 空的旧文件，不会被 CMake 自动识别
└── build/               # 执行配置命令后生成的构建目录
```

CMake 默认识别的文件名是 `CMakeLists.txt`，构建时使用该文件。
