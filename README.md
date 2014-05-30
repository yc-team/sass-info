sass-info
=========

#### 变量

* 全局还是局部？
* 什么时候有局部？


- 先看一段代码把：

```shell
$color: red;

h1 {
  color: $color;
}

p {
  $color: blue;
  color: $color;
}

span {
  color: $color;
}
```

转换后的代码：


```shell
h1 {
  color: red;
}

p {
  color: blue;
}

span {
  color: blue;
}

```


- 再看一段代码把


```shell
h1 {
  $color:blue;
  color: $color;
}

p {
  color: $color;
}
```

上面的代码会报错：

> Undefined variable: "$color".


我们来总结一下把：

1. 第一段代码里面看到，后面的p自己定义了变量color，后面会覆盖前面
2. 第二段代码里面看到，h1里面定义了变量color，p没有定义，就报错了

