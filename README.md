# 云上宫阙 · 中式梦核天上宫阙

一个可交互的 3D 中式梦核浮空宫阙：Blender 建模 + three.js 运行，含昼 / 昏 / 夜 / 雨四种天色、水母漫游、栈桥锦鲤、可进入的「揽月书斋」（题字、鉴宝、灯谜、烟花与拍照）。

## 部署到 GitHub Pages

1. 新建一个仓库（例如 `celestial-palace`），把本目录下的**所有文件**放到仓库根目录：

   ```
   index.html
   three-kit.js
   layout-data.js
   scene-data.js
   bgm-data.js
   font-data.js
   .nojekyll
   README.md
   ```

2. 提交推送：

   ```bash
   git add -A
   git commit -m "deploy celestial palace"
   git push origin main
   ```

3. 仓库 → Settings → Pages → Build and deployment：
   - Source 选 `Deploy from a branch`
   - Branch 选 `main`，目录选 `/ (root)`，保存

4. 等 1～2 分钟，访问 `https://<你的用户名>.github.io/<仓库名>/`。

## 说明

- 所有资源都是**相对路径**，可放在仓库根目录，也可放在任意子目录（如 `docs/`），不需要改代码。
- 全部资源随包下发，**不请求任何外部服务**；断网也能打开（音乐需点击一次后开始播放）。
- 文件较大（约 9.5 MB）：`scene-data.js`（3D 场景）、`font-data.js`（毛笔字体）、`bgm-data.js`（背景音乐）都是数据文件，请勿改动或重命名。
- 首次打开发送约 9.5 MB 数据，加载页会显示真实进度百分比。
- 若启用 HTTPS（GitHub Pages 默认是），所有能力均可用。
