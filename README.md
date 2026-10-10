# rxhaol.github.io

**这个仓库只是发布目标，请不要在这里改动任何东西。**

个人主页的**源码和文档全都在私有仓库 [`gh-pages.source`](https://github.com/rxhaol/gh-pages.source)** ——
改内容、写文章、部署，都在那边操作。

## 分支说明

| 分支 | 内容 |
| --- | --- |
| `main` | 只有这个说明文件（你正在看的） |
| `gh-pages` | 构建产物，由 Actions 自动更新，**不要手动改** |

## 部署方式

在 `gh-pages.source` 里执行一条命令即可：

```powershell
pnpm deploy "更新说明"
```

推送后 GitHub Actions 会自动构建，并把产物发布到本仓库的 `gh-pages` 分支。

- 站点地址：<https://rxhaol.github.io/>
- 构建进度：<https://github.com/rxhaol/gh-pages.source/actions>
- 部署目标配置：`gh-pages.source` 仓库里的 `deploy.config.json`

## 需要密钥

跨仓库推送需要 `gh-pages.source` 里配置名为 `DEPLOY_TOKEN` 的 Actions 密钥。
完整说明见 `gh-pages.source` 的 README「关于 Token 的安全性」。