# 恐龙跑酷 · 像素黑白

一款纯浏览器运行的黑白像素风恐龙跑酷小游戏。单文件、零外部依赖，开箱即玩，也适合托管到任何静态站点公开分享。

## ✨ 特性

- 🦖 像素霸王龙主角（大头 / 眼睛 / 小前肢 / 长尾 / 双腿奔跑动画）
- 🎮 流畅的跑动、跳跃、二连跳（空中可再跳一次）
- 🪙 以拾取金币计分：金币 +10 分
- ⭐ 随机道具：星星 +50 · 钻石 +100 · 皇冠 +500（稀有）· 磁铁（8 秒吸附金币）
- 🏆 历史记录（localStorage 本地保存），最高纪录以徽章高亮标记
- 📖 首页「道具图鉴」查看各道具作用与分值
- ⬛⬜ 严格黑白色调，像素字体 HUD，视差山丘与云层

## 🕹 操作

| 按键 / 操作 | 作用 |
| --- | --- |
| `Space` / `↑` / 点击屏幕 | 跳跃（空中可二连跳） |
| `↓` | 快速下落 |
| 长按跳跃键 | 跳得更高 |

## 🚀 本地运行

直接用浏览器打开 `index.html` 即可，无需安装任何依赖。

## 🌐 部署到 GitHub Pages（公开访问）

1. 注册 / 登录 <https://github.com>
2. 右上角 **+ → New repository**，名称填 `dino-runner`，选择 **Public**，点击 **Create repository**
3. 把本仓库文件上传进去，两种方式任选：

   **方式一：网页上传（最简单）**
   - 进入仓库 → **Add file → Upload files** → 把 `index.html`、`README.md`、`.nojekyll` 拖进去 → **Commit changes**

   **方式二：命令行推送（本仓库已初始化 git）**
   ```bash
   git remote add origin https://github.com/<你的用户名>/dino-runner.git
   git push -u origin main
   ```

4. 仓库页 **Settings → Pages**
   - Source 选 **Deploy from a branch**
   - Branch 选 `main`，目录选 `/ (root)`，点 **Save**
5. 等待约 1 分钟，访问 `https://<你的用户名>.github.io/dino-runner/` 即可公开游玩

> 历史记录与最高分保存在**每位玩家各自的浏览器**中（localStorage），无需服务器。

## 📁 文件说明

- `index.html` —— 游戏主体（含 HTML / CSS / JavaScript）
- `.nojekyll` —— 让 GitHub Pages 跳过 Jekyll 处理，按原样伺服
- `README.md` —— 本说明文档
