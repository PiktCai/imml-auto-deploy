# imml-auto-deploy
这是一个简单的项目，旨在使用 Github Actions 自动将使用 [imml](https://github.com/leoncvlt/imml) 语言编写的源文件转化为`.html`网页并部署到另一分支。  
## 什么是 imml？
>imml (indented markdown markup language，即“缩进式 markdown 标记语言”) 是一种标记语言，亦是一款静态网页生成器，旨在由一个单一便携的普通文本文件创建出极简极速且不含 Javascript 的网站。  
>本项目诞生自对于这样一种过程的追求：仅仅修改一个普通的文本文件，便能创建一个个人网站。它将是你托管博客、菜谱、公共大脑转储、简易作品集和低保真电子杂志等的不二之选，只有你想不到，没有它托管不了。  

更多介绍请前往[原项目](https://github.com/leoncvlt/imml)查看。
## 如何使用本项目？
- 点击`Use this template`使用此模板创建你的个人仓库
- 修改`index.imml`文件，在其中写入你想要的东西，具体格式可参考[编写细则（英文）](https://github.com/leoncvlt/imml/wiki/Writing-Guide)。
如此便大功告成，一旦你将修改推送至仓库的`main`分支， Github Actions 便会帮你完成剩下的事情，稍等片刻，构成网站的文件将会出现在`deploy`分支，届时你便可以根据自己的需要，选择不同的托管服务（如 Github Pages、Netlify 和 Vercel 等） 托管你的网站了！
## 注意事项
如果你不乐意使用`index.imml`作为文件名，你大可以将其修改，但是请同时把`.github/workflows/page_deploy.yml`文件中的步骤 2 和 3 中的文件名及输出目录一并修改，否则会导致运行报错。
## License
[MIT](https://github.com/PiktCai/imml-auto-deploy/blob/main/LICENSE) © PiktCai