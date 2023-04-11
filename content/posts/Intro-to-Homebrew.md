---
title: "Intro to Homebrew"
date: 2022-11-28T18:47:25-08:00
tags: [“Homebrew”]
Categories: ["Software"]
---

# 安装[Homebrew](https://brew.sh/)

打开终端，复制以下代码到终端，按回车即可：

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

| 词汇          | 含义                                                         |
| :------------ | :----------------------------------------------------------- |
| `formula (e)` | 安装包的描述文件，formulae 为复数                            |
| `cellar`      | 安装好后所在的目录                                           |
| `keg`         | 具体某个包所在的目录，keg 是 cellar 的子目录                 |
| `bottle`      | 预先编译好的包，不需要现场下载编译源码，速度会快很多；官方库中的包大多都是通过 bottle 方式安装 |
| `tap`         | 下载源，可以类比于 Linux 下的包管理器 repository             |
| `cask`        | 安装 macOS native 应用的扩展，你也可以理解为有图形化界面的应用。 |
| `bundle`      | 描述 Homebrew 依赖的扩展                                     |

| Command                   | Description                 |
| ------------------------- | --------------------------- |
| `brew search [关键词]`    | search software             |
| `brew install [软件名]`   | Install software            |
| `brew list`               | List all packages installed |
| `brew upgrade`            | upgrade software            |
| `brew uninstall [软件名]` | Uninstall software          |
| `brew info [软件名]`      | Get software info           |
| `brew cleanup`            | Clean up old software       |

# 管理后台软件

诸如 Nginx、MySQL 等软件，都是有一些服务端软件在后台运行，如果你希望对这些软件进行管理，可以使用 `brew services` 命令来进行管理

| Command                          | Description                     |
| -------------------------------- | ------------------------------- |
| `brew services list`             | Get services list               |
| `brew services run [服务名]`     | Run service                     |
| `brew services start [服务名]`   | Start service and set autostart |
| `brew services stop [服务名]`    | Stop service                    |
| `brew services restart [服务名]` | Restart service                 |

# Resource

- https://sspai.com/post/56009
