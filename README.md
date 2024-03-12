# 学习内容简述

## props

与data并列
可以用于接收外面传入的数据，并且限制类型

## computed

与data并列
容纳用于计算的函数，和methods里的相比相对简单

## v-bind数据单向绑定

用法：v-bind:class (后面属性是什么无所谓)
简写：:class

## v-model数据双向绑定

用法：v-model="label"
修饰符：
- .trim  删除空格
- .lazy  按表面意思理解：**懒得（更新）**
        只会在输入失去焦点或提交表单时同步数据

## v-on监听事件响应绑定

用法：v-on:click
简写：@click
注：这里不是click，而是其他事件，甚至是自定义事件都行

## v-for循环创建组件

类似python中的循环
eg. `v-for:"item in items"`

## $emit(expression)

将expression的内容传到父组件

## 箭头函数   =>

eg. 
```javascript
var hello;
hello = () => "Hello World!";
```
相当于
```javascript
 hello = function() {
     return "Hello World!";
 }
```

## uniqueID包

用于对组件的id进行**软编码**，在相应的后缀后面自动地编号
通常和v-for一起使用