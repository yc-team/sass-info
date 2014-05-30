sass-info
=========

#### 变量

* 全局还是局部？
* 什么时候有局部？


先看一段代码把：

```shell
$color: red;

h1 {
  color: $color;
}

p {
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
  color: red;
}

span {
  color: red;
}
```


