# SSPanel 自动签到

![SSPanel_Auto_Checkin](https://github.com/isecret/sspanel-autocheckin/workflows/SSPanel_Auto_Checkin/badge.svg)

> 注意：关于定时任务(cron)不执行的情况，你可能需要修改项目相关文件，比如这个 README.md，新增一个空格也算，然后提交就行。

## 使用方法

### 方式一：Github Actions（推荐）

Fork 该仓库，进入仓库后点击 `Settings`，右侧栏点击 `Secrets`，点击 `New secret`。分别添加 `DOMAIN`、`USERNAME` 和 `PASSWD` 的值，对应为你的 `域名`、`用户名` 和 `密码`。

定时任务将于每天凌晨 `2:20` 分执行，如果需要修改请编辑 `.github/workflows/work.yaml` 中 `on.schedule.cron` 的值（注意，该时间时区为国际标准时区，国内时间需要 -8 Hours）
