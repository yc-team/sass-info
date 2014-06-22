##记录一下颜色函数相关

#### rgb($red, $green, $blue)

根据红、绿、蓝三个值创建颜色

```shell
rgb(255, 0, 0);  //#ff0000
```

#### rgba($red, $green, $blue, $alpha)

根据红、绿、蓝和透明度创建颜色

```shell
rgba(#ff0000, 0.2);  //rgba(255, 0, 0, 0.2)
```

#### red($color)

从一个颜色值里面获取红色的值

```shell
red(#ff0000);  //255
```


#### green($color)

从一个颜色值里面获取绿色的值

```shell
green(#00ff00);  //255
```


#### blue($color)

从一个颜色值里面获取蓝色的值

```shell
blue(#0000ff);  //255
```

#### HSL

* H 色相
* S 饱和度： 0度是红色、120度是绿色、240度是蓝色
* L 亮度

下图来自w3cplus:

![HSL](http://cdn1.w3cplus.com/sites/default/files/styles/print_image/public/hsl_top.jpg)


