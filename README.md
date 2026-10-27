# Tools

一些纯前端的小工具，打开即用，数据不上传。

**在线地址**：https://pycv.github.io/tools/
**博客**：https://pycv.github.io/blog/

[![Deploy](https://img.shields.io/badge/GitHub%20Pages-live-2ea44f?logo=github)](https://pycv.github.io/tools/)

## 工具

| 工具 | 在线使用 | 说明 |
|------|----------|------|
| JSON 格式化 | [打开](https://pycv.github.io/tools/tools/json-formatter/) | 格式化、压缩、校验 JSON，报错带行列位置 |
| 时间戳转换 | [打开](https://pycv.github.io/tools/tools/timestamp/) | Unix 时间戳与本地时间、UTC、ISO 互转 |

## 特点

- 纯静态，无构建步骤、无后端依赖
- 所有处理都在浏览器本地完成，内容不会上传
- 支持深色模式，跟随系统

## 目录结构

```
.
├── index.html              # 导航页
├── 404.html
├── assets/style.css        # 共用样式
└── tools/<name>/index.html # 每个工具一个目录
```

## 新增一个工具

1. 新建 `tools/<name>/index.html`
2. 引入 `../../assets/style.css`，复用已有样式变量
3. 在根目录 `index.html` 的工具网格里加一张卡片
4. 更新本 README 的工具表
5. commit & push，GitHub Pages 自动发布（约 1 分钟）

## 本地预览

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000/
```

## 技术

原生 HTML / CSS / JavaScript，零运行时依赖。

## License

MIT
