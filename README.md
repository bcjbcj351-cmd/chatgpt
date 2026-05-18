# NEWOA 系统

这个仓库用于存放并后续开发 `NEWOA (3)(1).zip` 中的 OA / HR 系统代码。

## 原始文件

- 上传文件：`NEWOA (3)(1).zip`
- 用途：后续一起开发 OA / HR 系统

## 包内主要结构

```text
NEWOA/
├── backend/                 # FastAPI 后端
├── frontend/                # Vue 3 前端
├── android-recorder-app/    # Android 录音 / 面试相关 App
├── xyjrs/                   # 旧系统或参考资料
├── tmp/                     # 临时脚本与需求文档
├── README.md                # 原项目说明
└── PROGRESS.md              # 原项目进度说明
```

## 后续开发约定

1. 仓库目标：作为后续开发主仓库。
2. 核心原则：除 UI 调整外，不随意改变原系统业务流程和逻辑。
3. 优先方向：先跑通项目，再逐步补功能、修问题、做重构。
4. 安全原则：不要把真实 `.env`、密码、证书、签名文件、日志、构建产物直接放到公开仓库。

## 当前状态

当前连接器已连接到 GitHub，并确认目标仓库为：

```text
bcjbcj351-cmd/chatgpt
```
