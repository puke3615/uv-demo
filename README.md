# Weather CLI

一个简单的天气查询命令行工具。目前使用模拟数据来演示天气信息。

## 功能特点

- 支持查询任意城市的天气信息
- 使用模拟数据，无需API密钥
- 简单易用的命令行界面

## 安装方法

### 方法1：从PyPI安装（推荐）

```bash
# 使用pip
pip install puke3615-weather-cli

# 使用uv
uv pip install puke3615-weather-cli
```

### 方法2：直接运行（无需安装）

如果你安装了 `uv`，可以直接使用 `uvx` 运行，无需安装：

```bash
# 从PyPI运行（推荐）
uvx --from puke3615-weather-cli weather 北京

# 从GitHub运行
uvx --from git+https://github.com/puke3615/uv-demo.git weather 北京
```

### 方法3：从GitHub安装

```bash
# 使用uv
uv pip install git+https://github.com/puke3615/uv-demo.git

# 使用pip
pip install git+https://github.com/puke3615/uv-demo.git
```

### 方法4：本地安装

```bash
# 克隆仓库
git clone https://github.com/puke3615/uv-demo.git
cd uv-demo

# 使用uv安装
uv pip install -e .

# 使用pip安装
pip install -e .
```

## 使用方法

如果你通过方法1、3或4安装了包，你可以直接使用 `weather` 命令：

```bash
# 查询某个城市的天气
weather 北京

# 带API密钥的查询（当前版本会忽略该参数）
weather 上海 --api-key YOUR_API_KEY
```

如果你使用 `uvx` (方法2)，请参考上面的 `uvx` 命令格式。

## 示例输出

```
城市: 北京, 模拟国家
温度: 23.5°C
天气: 晴朗
风速: 15.5 km/h
湿度: 65%
```

## 开发说明

1. 克隆仓库
2. 创建并激活虚拟环境
3. 安装开发依赖

```bash
git clone https://github.com/puke3615/uv-demo.git
cd uv-demo
uv venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
uv pip install -e .
```

## 许可证

MIT License
