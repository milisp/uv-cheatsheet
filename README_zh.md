# uv-cheatsheet

以下是 `uv`（一个基于 Rust 编写的极快 Python 包和项目管理器）的简明速查表：  

---

### **安装**
- **macOS 和 Linux：**
  ```bash
  curl -LsSf https://astral.sh/uv/install.sh | sh
  ```
- **Windows：**
  ```powershell
  powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
  ```
- **使用 pip：**
  ```bash
  pip install uv
  ```

---

### **创建新项目**
初始化一个新 Python 项目：  
```bash
uv init my_project
cd my_project
```

---

### **依赖管理**
- **添加依赖：**
  ```bash
  uv add package_name
  ```
- **移除依赖：**
  ```bash
  uv remove package_name
  ```
- **升级依赖：**
  ```bash
  uv lock --upgrade-package package_name
  ```

---

### **运行脚本和命令**
- **运行 Python 脚本：**
  ```bash
  uv run script.py
  ```
- **在项目环境中执行命令：**
  ```bash
  uv run command
  ```

---

### **工具管理**
- **临时运行工具（无需安装）：**
  ```bash
  uvx tool_name
  ```
- **全局安装工具：**
  ```bash
  uv tool install tool_name
  ```

---

### **Python 版本管理**
- **安装指定的 Python 版本：**
  ```bash
  uv python install 3.10.5
  ```
- **设置项目的 Python 版本：**
  ```bash
  uv python local 3.10.5
  ```

---

### **构建与发布**
- **构建项目：**
  ```bash
  uv build
  ```
- **发布到 PyPI：**
  ```bash
  uv publish
  ```

---

### **缓存管理**
- **清理 uv 缓存：**
  ```bash
  uv cache clear
  ```

---

### **自我管理**
- **更新 uv 到最新版本：**
  ```bash
  uv self update
  ```

---

更详细的信息和进阶用法，请参考官方文档：[uv 文档](https://docs.astral.sh/uv/)。
