# node.js-angular6
使用node.js搭建以angularjs6为框架的工程结构


安装node.js及npm
npm config set registry https://registry.npm.taobao.org
安装angular cli
npm install -g @angular/cli
#添加eslint工具
npm install eslint -g
#webstorm配置eslint
1.进入File > Settings > Language & Frameworks > JavaScript > Code Quality Tools > ESLint面板，点选“Enable”进行如下配置：
2.在Node Interpreter字段中，指定Node.js的路径。如果您遵循标准安装过程，WebStorm会检测路径并填写字段本身。
3.在“ESLint包”字段中，指定eslint或标准包的位置（此处为eslint的文件夹目录）。
标准包的路径：C:\Users\cWX431487\AppData\Roaming\npm\node_modules\eslint
4.在项目根目录中创建.eslintrc文件，进行如下配置：
{
  "extends": "eslint:recommended",
  "env":{
    "node":true,
    "es6":true
  },
  "rules": {
    "semi": ["error", "always"],
    "quotes": "off",
    "no-console":"off",
    "no-unused-vars":"off",
    "no-unreachable":"off",
    "no-redeclare":"warn"
  }
}
5.点选"Search for .eslintrc"，WebStorm会查找.eslintrc文件或尝试检测package.json中eslintConfig下定义的配置。 WebStorm首先在包含要删除文件的文件夹中查找.eslintrc或package.json，然后在其父文件夹中查找，依此类推到项目根目录。如果搜索失败，ESLint将使用其默认的嵌入式配置文件。
6.完成配置
#wenstorm配置eslint相关可参考
https://www.jetbrains.com/help/webstorm/eslint.html
#eslint规则配置可参考
https://github.com/wy-ei/notebook/issues/36
