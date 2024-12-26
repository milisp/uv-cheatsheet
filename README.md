# uv-cheatsheet

Here's a concise cheatsheet for `uv`, an extremely fast Python package and project manager written in Rust.

**Installation**

- **macOS and Linux:**
  ```bash
  curl -LsSf https://astral.sh/uv/install.sh | sh
  ```
- **Windows:**
  ```powershell
  powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
  ```
- **Using pip:**
  ```bash
  pip install uv
  ```

**Creating a New Project**

Initialize a new Python project:
```bash
uv init my_project
cd my_project
```

**Managing Dependencies**

- **Add a dependency:**
  ```bash
  uv add package_name
  ```
- **Remove a dependency:**
  ```bash
  uv remove package_name
  ```
- **Upgrade a dependency:**
  ```bash
  uv lock --upgrade-package package_name
  ```

**Running Scripts and Commands**

- **Run a Python script:**
  ```bash
  uv run script.py
  ```
- **Execute a command within the project environment:**
  ```bash
  uv run command
  ```

**Tool Management**

- **Run a tool without installing (ephemeral environment):**
  ```bash
  uvx tool_name
  ```
- **Install a tool globally:**
  ```bash
  uv tool install tool_name
  ```

**Python Version Management**

- **Install a specific Python version:**
  ```bash
  uv python install 3.10.5
  ```
- **Set the project's Python version:**
  ```bash
  uv python local 3.10.5
  ```

**Building and Publishing Packages**

- **Build the project:**
  ```bash
  uv build
  ```
- **Publish to PyPI:**
  ```bash
  uv publish
  ```

**Cache Management**

- **Clear uv's cache:**
  ```bash
  uv cache clear
  ```

**Self-Management**

- **Update uv to the latest version:**
  ```bash
  uv self update
  ```

For more detailed information and advanced usage, refer to the official [uv documentation](https://docs.astral.sh/uv/). 
