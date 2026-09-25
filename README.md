# 《造化笔》安装包发布仓库

这里是《造化笔》的安装包发布仓库：**只放安装包与 SHA256 校验和，不含源码**（源码仓库暂不公开）。

## 下载安装

1. 到 [Releases](https://github.com/bshilm/zaohuabi-releases/releases) 选最新版本，下载 `ZaoHuaBi-<版本>-win-x64.exe`；
2. 双击安装（未做代码签名，SmartScreen 可能提示「未知发布者」→「更多信息」→「仍要运行」）；
3. 安装包旁的 `SHA256SUMS.txt` 可用来校验下载是否完整。

## 应用内更新

软件「设置 → 关于与性能 → 更新与备份」里的**更新源地址**默认为：

    https://api.github.com/repos/bshilm/zaohuabi-releases/releases

这是公开仓库，**不需要访问令牌**；点「手动检查更新」即可检查 → 下载 → 安装并重启。
升级前会自动把整个书夹备份到书夹旁的 `_zaohuabi_backup/upgrade_v<旧>_to_v<新>_<时间戳>`。

## 版本说明

每个 Release 的说明（body）就是该版本的更新说明，也可在应用的更新卡片里直接看到。

---

本仓库由 `npm run release -- --publish` 自动发布。
