# RustMinerSystem 定制安装入口

本仓库只保存客户安装脚本和公开版本清单。Linux、Windows 程序及历史版本由 Cloudflare R2 托管，下载域名为 `https://shortcut.rustminersystem.com`。

- `Readme/<CID>/install.sh`：客户安装脚本。保留原路径及 Git LFS，现有 `media.githubusercontent.com/media/EvilGenius-dot/shortcut/main/Readme/<CID>/install.sh` 安装命令继续有效。
- `releases/<CID>.json`：官网定制查询使用的普通 Git JSON，记录当前版本、历史版本、R2 对象路径、大小与 SHA-256。

发布新版本时，在编译发布工具选择「R2 定制发布」。工具从当前版本的归集目录读取程序，上传并完成公网校验后，更新本仓库的脚本和清单；检查后提交、推送即可。

历史程序在 R2 中保留，不需要把二进制复制进本仓库。已有发布清单必须随仓库保留，以便后续发布继承历史下载记录。
