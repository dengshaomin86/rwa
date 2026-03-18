# rwa
rwa preview

## q
```
1. /assets/_plugin-vue_export-helper-DlAUqK2U.js 响应 404
这通常是因为 GitHub Pages 默认使用 Jekyll 作为静态网站生成引擎，而 Jekyll 有一个安全策略：会自动忽略以点（.）或下划线（_）开头的目录和文件。

由于 Vite 在打包时可能会生成类似 _plugin-vue_export-helper 的文件，导致 GitHub Pages 找不到这些资源。

解决方案：添加 .nojekyll 文件
要解决这个问题，你需要告诉 GitHub Pages 禁用 Jekyll 引擎，直接作为普通静态文件托管。

操作步骤：
在你的项目根目录（或者你的 public 目录下）创建一个名为 .nojekyll 的空文件（注意文件名开头有一个点）。

确保这个文件被提交并推送到 GitHub 仓库的部署分支（通常是 gh-pages 或 main）。

重新发布后，GitHub Pages 将不再过滤掉下划线开头的文件。
```
