# Deploy Notes

这个网站已经改成了静态可部署版本，文件之间使用相对路径。

## 目录

- `index.html`
- `resume-online.html`
- `project-househelp.html`
- `avatar.jpg`
- `徐龙威-个人简历-更新版.docx`

## 安全边界

别人可以访问网站，不代表别人可以修改网站。

只有你能修改的前提是：

1. 网站文件放在你自己的 GitHub 仓库里
2. 只有你的 GitHub 账号有仓库写权限
3. 部署平台绑定你的账号
4. 你的账号开启两步验证 `2FA`

## GitHub Pages

1. 新建一个你自己的仓库
2. 把这个目录下的全部文件上传到仓库根目录
3. 在仓库 `Settings -> Pages` 中启用 GitHub Pages
4. `Source` 选择部署分支，例如 `main`
5. 保存后等待发布

## Vercel

1. 用你自己的 GitHub 账号登录 Vercel
2. 导入这个仓库
3. Framework 选 `Other`
4. Root Directory 设为当前网站目录
5. 直接部署

## 更新内容

以后你每次更新简历或页面，只需要：

1. 先改本地文件
2. 提交到你自己的仓库
3. 推送后平台会自动重新发布

## 提醒

- 不要把仓库写权限给别人
- 不要把 GitHub / Vercel 账号借给别人
- 最好开启 `2FA`
