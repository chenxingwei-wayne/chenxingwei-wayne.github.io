npm install在安装node模块时，有两种命令参数可以把它们的信息写入package.json文件：
–save
–save-dev

但它的文档里1，只提到一个小区别，–save会把依赖包名称添加到package.json文件dependencies键下，–save-dev则添加到package.json文件devDependencies键下

如果你将包下载下来在包的根目录里运行,执行如下命令,默认会安装两种依赖
npm install

如果你只是单纯的使用这个包而不需要进行一些改动测试之类的，只安装dependencies而不安装devDependencies。执行：
npm install --production

通过“npm install packagename”进行安装，只会安装dependencies
npm install packagename

如需安装devDependencies，执行：
npm install packagename --dev
