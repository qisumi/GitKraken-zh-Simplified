# GitKraken 简体中文翻译

[GitKraken](https://www.gitkraken.com/) 简体中文翻译补丁，主要将[这个项目](https://github.com/rogeraabbccdd/GitKraken-zh-tw)的繁体中文翻译简体化，目前还未完全完成。主要做出如下修改：

1. 将繁体文字简体化
2. 将部分的原作者符合繁体表达的词组进行简体化，例如：
   1. submit --> 送出 --> 提交
   2. custom --> 自订 --> 自定义
   3. file --> 资料档 --> 文件
3. 将部分的词组取消翻译，例如：
   1. Hooks --> 拉钩 --> Hooks

## 使用方法

- 目前支持版本：9.0.1
- 下载`strings.json`
- 覆盖文件
  - Windows: `%LOCALAPPDATA%\gitkraken\app-9.0.1\resources\app.asar.unpacked\src\strings.json`
  - Mac: `/Applications/GitKraken.app/Contents/Resources/app.asar.unpacked/src/strings.json`
  - Linux: `/usr/share/gitkraken/resources/app.asar.unpacked/src`

- 重新启动`GitKraken`，至`Preference -> UI Customization -> Language`切换语言。

## 更新翻译文件格式

新版本的`GitKraken`发布时，使用`update.js`将翻译档更新为新版本格式。

- 安裝 [Node.js](https://nodejs.org/en/)
- 下载 `update.js` 到翻译目录
- 将新版的英文 `strings.json` 重新命名为 `strings.en.json`
- 将未更新的中文翻译文件 `strings.json` 放入目录
- 用终端执行 `node update.js`