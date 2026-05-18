# 清理报告

本目录从 `NEWOA (3)(1).zip` 解压清理而来，保留源码、配置模板和开发文档，删除或替换了不适合进入公开 Git 仓库的内容。

## 已删除/排除

- 第三方二进制工具：`.tools/putty/`
- AI/本地助手过程目录：`.claude/`、`.workbuddy/`
- 部署临时脚本：`.deploy_do.py`、`.deploy_fix.py`、`.deploy_probe.py`、`_deploy.py`、`_remote_exec.py`
- 构建/发布包：`frontend-dist-*.zip`、`backend-upload-*.zip`
- Python 缓存：`__pycache__/`、`*.pyc`
- 运行日志：`*.log`
- 真实环境变量：`backend/.env`、`frontend/.env.*`
- Android 本机/签名配置：`local.properties`、`keystore.properties`、`*.keystore`

## 已替换为模板

- `backend/.env.example`
- `frontend/.env.development.example`
- `frontend/.env.production.example`
- `android-recorder-app/keystore.properties.example`

## 保留内容

- `backend/`：FastAPI 后端源码、迁移、脚本
- `frontend/`：Vue 3 前端源码、配置、锁文件
- `android-recorder-app/`：Android 源码、Gradle 配置
- `xyjrs/`：旧系统/参考资料
- `tmp/`：需求与测试脚本
- `README.md`、`PROGRESS.md`、`CLAUDE.md`

## 清理后规模

- 保留文件数：约 287 个
- 源码目录大小：约 2.7MB
- 清理后压缩包大小：约 616KB

## 本地测试前需要补齐

1. 根据 `backend/.env.example` 创建 `backend/.env`。
2. 根据 `frontend/.env.development.example` 创建 `frontend/.env.development`。
3. 如需 Android 打包签名，根据 `android-recorder-app/keystore.properties.example` 在本地创建真实 `keystore.properties`。
4. 不要把真实密码、签名文件、服务器地址、部署脚本提交到公开仓库。
