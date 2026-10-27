# tools

一些纯前端的小工具，打开即用，数据不上传。

线上地址：https://pycv.github.io/tools/

## 工具列表

| 工具 | 路径 | 说明 |
|------|------|------|
| JSON 格式化 | `/tools/json-formatter/` | 格式化、压缩、校验 JSON |
| 时间戳转换 | `/tools/timestamp/` | Unix 时间戳与本地/UTC/ISO 互转 |

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
3. 在 `index.html` 的工具网格里加一张卡片
4. commit & push，GitHub Pages 自动生效（分支部署，无需 CI）

## 约定

- 纯静态，不引入构建步骤和后端依赖
- 所有数据处理留在浏览器本地
- 相对路径引用资源，方便本地直接打开预览
