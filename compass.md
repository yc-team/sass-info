## 介绍一些compass命令相关的

#### 如何初始化？

```shell
compass creat myproject
```

会生成一个myproject的子目录，包含：

- config.rb
- sass
- stylesheets


#### 如何编译？

* 一次性编译

```shell
compass compile
```

在项目根目录下运行，会将sass目录的scss文件，编译成css文件，保存到stylesheets目录中

> compass一般只编译改动的文件，如果需要把所有文件都编译，增加参数 --force


* 自动编译

```shell
compass watch
```

只有scss文件有修改，就会自己编译
