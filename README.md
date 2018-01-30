# myWebpack

webpack.config.js 主要配置项，
  出口（entry）、
  入口（output）、
  插件（plugins）
  
 其次是对于module模块化处理的配置
 
1、配置路径用path.resolve()处理，为了确保路径是从根目录开始绝对定位到指定位置，webpack3.0要求我们在配置路径相关的时候使用绝对路径；
2、path模块是nodejs内置的处理路径相关的模块。

devServer: {
    port: 3000, // 这个是热启动的端口
    inline: true
}
 
************************************************************************************
"scripts": {
    "server": "node server.js", // 启动服务器
    "build": "webpack", // 打包命令
    "dev": "webpack-dev-server" // 热启动服务器
}

内置一个 express 服务器

************************************************************************************
安装的webpack插件

1、安装根据模板动态生成Html
命令：npm install html-webpack-plugin --save-dev

2、清除打包文件夹下面的重复文件
命令：npm install clean-webpack-plugin --save-dev

3、安装css-loader和style-loader
命令：npm install style-loader css-loader --save-dev

4、postcss提供用来自动处理css在不同浏览器之间前缀等问题，使用autoprefixer需要先引入postcss。
命令：npm install postcss-loader autoprefixer --save-dev

5、babel-preset-env编译ES6
命令：npm install babel-loader babel-core babel-preset-env --save-dev

6、静态资源处理器extract-text-webpack-plugin
命令：npm install extract-text-webpack-plugin --save-dev  
脚手架没有安装

7、url-loader 图片等其他资源加载器
命令：npm install url-loader --save-dev

8、image-webpack-loader 图片压缩
命令：npm install image-webpack-loader --save-dev

9、安装express服务器
命令：npm install express --save-dev

10、webpack-dev-server 服务器
命令：npm install webpack-dev-server --save-dev
