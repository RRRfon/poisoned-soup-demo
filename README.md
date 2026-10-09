# poisoned-soup-demo

《毒汤》网页试玩的公开部署仓库，仅存放 Godot Web 导出文件及发布配置。开发源码在独立私有仓库维护。

默认从图书馆序章开始，接续当前已完成的主线调查片段；这不是完整游戏。`?opening=1` 可直接测试主线，`?prototype=1` 保留独立的旧交互原型。

## 部署

在仓库 Settings → Pages 中，将 Source 设为 **GitHub Actions**。推送 main 或手动运行 Publish playable demo website 工作流，会将 `site/` 发布到 Pages。

## 本地查看

```bash
python -m http.server 8060 --directory site
```

打开 `http://localhost:8060/`。存档使用当前站点的浏览器存储，清除网站数据会删除存档。

## 许可证

Godot 引擎为 MIT 许可，见 `site/LICENSE-Godot.txt`；PrototypeSans／PrototypeSerif 字体子集源自 Noto CJK，遵循 SIL OFL 1.1，见 `site/LICENSE-Noto-CJK.txt`。
