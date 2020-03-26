# efox-cli脚手架模板库
本代码库用于存储 efox-cli 脚手架构建所用到的项目,通过映射管理各项目组维护的模板代码
## 1. 项目结构

### master
- `config.json`: 用于配置cli中模板的选项

  * `projects`:该对象存入的是`https://github.com/DIVINER-onlys`下的项目组名称(`name`值支持自定义，`value`值必须与对应项目组名称相同)。该对象信息用于`efox-cli`建立种子项目时提供的项目组选项。
```
{
  "projects": [
    {
      "name": "webpack",
      "value": "webpack"
    },
    {
      "name": "flutterBlog",
      "value": "flutterBlog"
    }
  ]
}
```

## 2. 使用 efox-cli 生成模板项目
### 安装
执行 `npm i -g efox-cli` 安装efox-cli脚手架
```
npm i -g efox-cli
```

尝试执行`efox-cli`，显示如下，就是安装成功了

![efox-cli](https://s1.ax1x.com/2020/03/20/8clrhd.png)

### 获取帮助
执行`efox-cli --help`或者`efox-cli create --help`获得相关帮助

<!-- ![efox-cli help](https://s1.ax1x.com/2020/03/20/8clw7D.png) -->

### 获取系统配置
执行`efox-cli info`获取系统配置

<!-- ![efox-cli info](https://s1.ax1x.com/2020/03/20/8clBAe.md.png) -->


### 开始使用
尝试生成一个种子项目，切换到种子项目要存放的路径下

* 按照`efox-cli 帮助`执行`efox-cli c test-app`

<!-- ![efox-cli create](https://s1.ax1x.com/2020/03/20/8clNX6.png) -->

* 这里会有一些选项，使用`方向键上/下`来选择不同项目，这里尝试选择`efox`

<!-- ![efox-cli create](https://s1.ax1x.com/2020/03/20/8cld0O.png) -->

<!-- * 这里可以选自己需要的模板代码，`方向键上/下`选择`nextjs` -->

<!-- ![efox-cli create](https://s1.ax1x.com/2020/03/20/8cl61I.png) -->

* 尝试打开我们建立的项目`test-app`目录，就能看到我们拉取的种子项目内容

恭喜完成！！！！

### 直接拉取种子项目
直接执行`efox-cli c test-app -p efox -m nextjs`
* c 创建项目指令
* test-app 即将创建的项目名称
* -p 指定项目组为efox
* -m 指定项目组下的模块为nextjs



