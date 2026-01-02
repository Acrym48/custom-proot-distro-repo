# 自定义 Proot Distro 仓库

各种 Linux 发行版的 Proot Distro 配置集合。该仓库提供了易于安装的配置，可以与 Termux 的 `proot-distro` 命令一起使用。

## 什么是 Proot Distro？

Proot Distro 是一个用于 Termux 的工具，可以轻松安装和管理各种 Linux 发行版的 chroot 环境。它允许您在不需给设备 root 的情况下运行原生 GNU/Linux 发行版。

## 安装

要安装此仓库中的配置：

```bash
# 克隆仓库
git clone https://github.com/yourusername/My-proot-distro-repo.git
cd My-proot-distro-repo

# 运行安装脚本
./install.sh
```

安装脚本会将 `distros` 目录中的所有配置文件复制到 `$PREFIX/etc/proot-distro/`。

## 使用

安装后，您可以使用以下命令来使用已安装的发行版：

```bash
# 列出可用的发行版
proot-distro list

# 安装发行版（示例）
proot-distro install <发行版名称>

# 登录到发行版（示例）
proot-distro login <发行版名称>
```

## 贡献

如果您想贡献新的发行版配置：

1. 在 `distros` 目录中创建新的配置文件
2. 遵循现有格式和约定
3. 提交前测试配置
4. 提交拉取请求

## 目录结构

- `distros/` - 包含发行版配置文件
- `install.sh` - 安装脚本
- `README.md` - 此文件
- `LICENSE` - 许可证信息

## 许可证

该项目根据 MIT 许可证授权 - 请参阅 [LICENSE](LICENSE) 文件了解详情。