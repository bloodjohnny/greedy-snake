# GreedySnake 项目云盘说明

## 项目地址

GitHub 仓库：`https://github.com/bloodjohnny/greedy-snake`
公网访问：`https://bloodjohnny.github.io/greedy-snake/`

## 换 PC 后如何继续

### 第一步：克隆项目到本地

```bash
git clone https://github.com/bloodjohnny/greedy-snake.git
cd greedy-snake
```

### 第二步：用本地 HTTP 服务打开

```bash
# Python 3
python3 -m http.server 8000
# 然后访问 http://localhost:8000
```

### 第三步：修改后推送更新

```bash
git add -A
git commit -m "描述你的修改"
git push origin master
```

推送后 GitHub Pages 会自动重新构建，约 1-2 分钟生效。

## 项目结构

```
greedy-snake/
├── index.html          # 游戏主文件（单文件，包含所有 CSS/JS）
└── assets/
    ├── tile.png     # 背景格子
    ├── snake-head.png
    ├── snake-body.png
    ├── snake-tail.png
    └── food.png
```

## 注意事项

- 游戏是**单文件**（`index.html`），CSS 和 JS 全内联，直接编辑这个文件即可
- GitHub Pages 构建需要 1-2 分钟，推送后稍等再刷新公网链接
- `assets/` 里的图片如果修改，记得 `git add` 后再提交
- `server.log` 是本地临时文件，不要提交

## 如需在沙盒环境继续

直接打开 CodeBuddy，项目会自动从关联的云盘加载 `/workspace` 内容。
