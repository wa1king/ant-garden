# 蚁径花园

在 46 × 40 的花卉棋盘上，指挥蚂蚁搬走同色方块。点击底部第一排色块，蚂蚁会逐只出洞。暂时够不到目标的一组会留在上方，等其他蚂蚁清出路线。

## 试玩与开发

直接用浏览器打开 `docs/index.html`。两个关卡、画面和音效都在这一个文件里，可以离线运行。

编辑 `src/` 下的源码后，在项目根目录运行 `python tools/build.py`，重新生成 `docs/index.html`。构建只使用 Python 3.10+ 标准库。棋盘数据和音效可以分别用 `src/boards/generate_boards.py` 与 `src/audio/synthesize.py` 重新生成。棋盘生成脚本需要 NumPy 和 Pillow。

## 发布到 GitHub Pages

推送 `main` 分支后，在 GitHub 仓库的 **Settings → Pages** 选择 **Deploy from a branch**，设置为 `main` 的 `/docs` 目录并保存。之后推送更新的 `docs/index.html` 即可更新游戏。

[GitHub Pages 发布设置](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
