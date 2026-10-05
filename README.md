# poisoned-soup-demo

《毒汤》无剧透交互原型的公开网页部署仓库，仅存放 Godot Web 导出文件及发布配置。开发源码在独立私有仓库维护。

这是技术验证场景，包含视角切换、调查、对话、物品、D100 检定与手动存档，不包含正式模组剧情。

## 部署

在仓库 Settings → Pages 中，将 Source 设为 **GitHub Actions**。推送 main 或手动运行 Publish prototype website 工作流，会将 `site/` 发布到 Pages。

## 本地查看

```bash
python -m http.server 8060 --directory site
```

打开 `http://localhost:8060/`。存档使用当前站点的浏览器存储，清除网站数据会删除存档。

## 许可证

Godot 引擎为 MIT 许可，见 `site/LICENSE-Godot.txt`；PrototypeSans 字体子集源自 Noto CJK，遵循 SIL OFL 1.1，见 `site/LICENSE-Noto-CJK.txt`。
