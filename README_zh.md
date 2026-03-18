# Ghostty Setup

一个美观且实用的 Ghostty 终端配置，搭配 Starship 提示符和 Catppuccin Macchiato 主题。

## ✨ 功能特性

- 🎨 使用 Catppuccin Macchiato 主题
- 💫 Starship 提示符（包含 Git、目录、时间、多语言支持等）
- 📝 Fira Code 字体
- 🌓 自动切换明暗主题
- 🪟 半透明毛玻璃效果
- ⚡ Quake 风格下拉终端
- ⌨️ 丰富的快捷键支持
- 🐟 配置为使用 fish shell（可自行修改）

## 🖼️ 截图

![Ghostty 终端截图](./media/09d1b4947d1f7f9b23cfcfb6a3c55505.png)

## 📦 前置条件

- 已安装 [Homebrew](https://brew.sh/)
- 已安装 Ghostty 终端
- （可选）已安装 fish shell

## 🚀 安装

### 1. 安装 Starship

```shell
brew install starship
```

### 2. 下载配置文件

```shell
# 创建配置目录
mkdir -p ~/.config/ghostty

# 下载 Ghostty 配置
curl -o ~/.config/ghostty/config https://raw.githubusercontent.com/BriceLucifer/ghostty_setup/refs/heads/main/config

# 下载 Starship 配置
curl -o ~/.config/starship.toml https://raw.githubusercontent.com/BriceLucifer/ghostty_setup/refs/heads/main/starship.toml
```

### 3. 配置 Starship（如果还没配置）

在你的 shell 配置文件（如 `~/.bashrc`、`~/.zshrc` 或 `~/.config/fish/config.fish`）中添加：

**Fish:**
```fish
starship init fish | source
```

**Zsh:**
```zsh
eval "$(starship init zsh)"
```

**Bash:**
```bash
eval "$(starship init bash)"
```

## ⌨️ 快捷键

| 功能 | 快捷键 |
|------|--------|
| 新建标签页 | `Cmd + T` |
| 关闭标签页/分屏 | `Cmd + W` |
| 左右切换标签页 | `Cmd + Shift + H/l` |
| 垂直分屏 | `Cmd + D` |
| 水平分屏 | `Cmd + Shift + D` |
| 分屏间导航 | `Alt + H/J/K/L` |
| 增大/减小字体 | `Cmd + +/-` |
| 重置字体大小 | `Cmd + 0` |
| 切换下拉终端 | ``Ctrl+` `` |
| 重载配置 | `Cmd + Shift + ,` |

## 📝 配置说明

### Ghostty 配置
- 字体：Fira Code，16px
- 主题：Catppuccin Macchiato（自动跟随系统）
- 背景：90% 透明度 + 20px 模糊
- 光标：闪烁块样式，自动反色

### Starship 配置
- 使用 Catppuccin Mocha 配色
- 支持多语言指示器（C、Rust、Go、Node.js、PHP、Java、Kotlin、Haskell、Python 等）
- 显示 Git 分支和状态
- 显示当前时间和命令执行时间

## 🎨 自定义

你可以根据需要修改 `~/.config/ghostty/config` 和 `~/.config/starship.toml` 文件来调整配置。

---

*享受你的新终端体验！* 🎉
