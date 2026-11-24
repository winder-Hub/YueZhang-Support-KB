# 月章智能客服知识库

这是月章（YueZhangio）智能客服「小月」使用的公开知识库，维护访客常见问题的标准答案。

## 文件结构

- `index.json`：知识库清单；新增文件时同步加入 `files`。
- `00-identity.md`：月章与三个世界。
- `01-account.md`：账号、注册、登录与找回密码。
- `02-yuehua.md`：月华与交易。
- `03-support.md`：客服渠道、服务时间与转人工规则。
- `04-feedback-partnership.md`：建言板、商务合作与加入我们。
- `05-policies.md`：安全、隐私与能力边界。
- `06-faq.md`：常见问答。

## 维护方式

1. 直接编辑 Markdown，保持中文、短句、可执行。
2. 新增文件时更新 `index.json` 的 `files` 数组；每次修改内容时递增 `index.json` 的 `version`，线上服务只会接受版本号不低于本地快照的远程知识库。
3. 不要写入密码、令牌、密钥、内部服务器地址或任何个人信息。
4. 提交到 `main` 分支。线上服务会定期通过 jsDelivr 从本仓库刷新；本地内置快照作为回退。月章服务器无法直接访问 GitHub raw，因此不要改用 raw.githubusercontent.com。

## 相关

- 主站：https://yuezhangio.com
- 客服页：https://yuezhangio.com/versions/1/support/
- 线上服务代码在主站仓库的 `server/support-agent/` 中维护。
