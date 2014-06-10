记录一些sass的function

#### 数字函数

* percentage($value)

```shell
.test {
	width: percentage(.3);
}
```

代码编译后：

```shell
.test {
  width: 30%;
}
```

* round()

做四舍五入，取一个最接近的整数

```shell
.test {
	width: round(10.4px);
}
.test1 {
	width: round(10.6px);
}
```

代码编译后：

```shell
.test {
  width: 10px;
}

.test1 {
  width: 11px;
}
```


* ceil()

返回一个 >= 自己的最接近的整数

```shell
.test {
	width: ceil(10.6px);
}
.test1 {
	width: ceil(10.1px);
}
```

代码编译后：

```shell
.test {
  width: 11px;
}

.test1 {
  width: 11px;
}
```


* floor()


返回一个 <= 自己的最接近的整数

```shell
.test {
	width: floor(10.6px);
}
.test1 {
	width: floor(10.1px);
}
```

代码编译后：

```shell
.test {
  width: 10px;
}

.test1 {
  width: 10px;
}
```


* abs()

取绝对值

```shell
.test {
	width: abs(-10px);
}
```

代码编译后：

```shell
.test {
	width: 10px;
}
```


* min()

任意多个参数中最小的

```shell
.test {
	width: min(10px ,1px ,20px);
}
```

代码编译后：

```shell
.test {
  width: 1px;
}
```

* max()

任意多个参数中最大的

```shell
.test {
	width: max(10px ,1px ,20px);
}
```

代码编译后：

```shell
.test {
  width: 20px;
}
```

