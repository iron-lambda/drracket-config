# DrRacket Config

[English](README.md) | [中文](README.zh-CN.md)

为 DrRacket 提供现代化键绑定配置，支持 REPL 集成。提供 Emacs 风格的增量求值功能——无需离开编辑器即可将表达式和选区直接发送到 REPL。

## 功能

- **发送代码到 REPL** — Emacs 风格的增量求值
  - 发送当前顶层表达式
  - 发送选中的代码区域
  - 可选择在发送后自动聚焦到 REPL 面板

## 环境要求

- DrRacket 7.0 或更高版本

## 安装

1. 克隆本仓库：

```bash
git clone https://github.com/jrtxio/drracket-config.git
```

2. 在 DrRacket 中：
   - 进入 **Edit** → **Keybindings** → **Add User-defined Keybindings...**
   - 选择克隆目录中的 `drracket-keybindings.rkt`
   - 重启 DrRacket

## 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl+C, Ctrl+E` | 发送当前表达式到 REPL |
| `Ctrl+C, Ctrl+R` | 发送选中代码到 REPL |
| `Ctrl+C, Alt+E` | 发送表达式并聚焦 REPL |
| `Ctrl+C, Alt+R` | 发送选中代码并聚焦 REPL |

**使用方法：**

- 将光标放在某个表达式内部或附近
- 按 `Ctrl+C` 然后按 `Ctrl+E` 在 REPL 中求值
- 或选中代码后按 `Ctrl+C` 然后按 `Ctrl+R`

**注意：** 使用前需先运行一次程序（F5）以初始化 REPL。

## 小提示

- **查看所有活跃的快捷键：** Edit → Keybindings → Show Active Keybindings

## 更新

```bash
cd /path/to/drracket-config
git pull
```

然后重启 DrRacket。

## 许可证

[MIT](LICENSE)
