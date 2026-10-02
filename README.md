# 尘世命轨 BGM 曲库

曲库使用 `manifest.json` 作为检索表，音频文件放在 `audio/` 目录。清单中的音频地址均相对于 manifest，因此移动仓库时不需要逐首改成本机绝对路径。

## 接入播放器

仓库上传后，复制 GitHub 上 `manifest.json` 的 **Raw** 地址，在播放器唯一的曲库地址输入框中填写该地址并加载。地址形式如下：

`https://raw.githubusercontent.com/<owner>/<repository>/<branch>/manifest.json`

音频文件会按清单中的 `audio/...` 路径从同一仓库读取。请使用实际仓库所有者、仓库名和分支替换尖括号内容。

## 用 GitHub Desktop 上传

1. 在 GitHub Desktop 中添加已有仓库，选择本目录。
2. 检查变更列表，确认包含 `manifest.json`、`README.md`、`.gitignore` 和 `audio/` 中的曲目。
3. 提交到本地后，再按需发布仓库；发布前建议先设为 Private。
4. 发布后打开 GitHub 上的 `manifest.json`，选择 Raw 并复制地址，填入播放器。

本机仓库已配置 `origin` 远端。此整理不会替你创建提交或推送。

## 音频授权

曲目的公开传播和再分发授权尚未逐首核实。请在确认授权前保持仓库私有；不要因为曲目已能播放就推断其可公开分发。
