
```markdown
# CMake 项目模板

这是一个基于 CMake 的 C++ 项目模板，适用于快速启动新项目。项目结构清晰，支持模块化开发、单元测试和跨平台构建。

## 项目结构

```plaintext
cmake_init/
├── build/           # 构建目录（不提交到 Git）
├── CMakeLists.txt   # CMake 主配置文件
├── include/         # 公共头文件目录
│   └── .gitkeep     # 用于跟踪空目录
├── src/             # 源代码目录
│   └── main.cpp     # 主程序入口
├── tests/           # 单元测试目录
│   └── .gitkeep     # 用于跟踪空目录
└── README.md        # 项目说明文档
```

## 快速开始

### 1. 克隆项目

```bash
git clone https://github.com/611711Dark/cmake_init.git
cd cmake_init
```

### 2. 配置和构建

1. 创建构建目录并运行 CMake：
   ```bash
   mkdir build
   cd build
   cmake ..
   ```

2. 编译项目：
   ```bash
   cmake --build .
   ```

3. 运行生成的可执行文件：
   ```bash
   ./my_app
   ```

### 3. 添加新模块

1. 在 `src/` 目录中添加新的 `.cpp` 文件。
2. 在 `include/` 目录中添加新的头文件。
3. 更新 `CMakeLists.txt`，确保新文件被包含在构建中。

### 4. 运行单元测试

1. 在 `tests/` 目录中添加测试代码。
2. 启用测试支持（在 `CMakeLists.txt` 中取消注释 `enable_testing()`）。
3. 构建并运行测试：
   ```bash
   cd build
   cmake --build .
   ctest
   ```

## 依赖项

- **CMake**: 最低版本 3.10
- **C++ 编译器**: 支持 C++17 或更高版本



