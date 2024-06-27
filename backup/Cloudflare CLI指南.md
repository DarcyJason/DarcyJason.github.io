# 使用Cloudflare（CLI）搭建Web应用
## 1.安装
根据官网安装Wrangler

## 2.认证
首先创建个人API TOKEN，复制下来并保存在你认为比较安全的地方，因为其API TOKEN无法进行二次查看，请一定妥善保管

再打开本地终端应用
`export CLOUDFLARE_API_TOKEN=YOUR_API_TOKEN`

如果你使用的是Bash，则输入以下命令
`echo 'export CLOUDFLARE_API_TOKEN=YOUR_API_TOKEN' >> ~/.bashrc`
`source ~/.bashrc`

如果你使用的是Zsh，则输入以下命令
`echo 'export CLOUDFLARE_API_TOKEN=YOUR_API_TOKEN' >> ~/.zshrc`
`source ~/.zshrc`

**将以上命令中的YOUR_API_TOKEN全都替换成你刚创建的API TOKEN**

## 3.使用
输入`npm create cloudflare@latest`命令，根据其提示信息选择并搭建你的Web框架应用，并将其部署到Cloudflare上

## 4.更新（以vue框架的web为例）
进入你本地的wrangler项目中，输入`npm run build`命令后，只需再输入`wrangler pages deploy ./dist`后，便可以更新你部署的网站