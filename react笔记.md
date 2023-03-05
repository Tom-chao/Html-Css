# react

### 虚拟DOM的两种创建方式

1.使用jsx

```js
#先引入
<script src="https://unpkg.com/react@17/umd/react.development.js" crossorigin></script>
<script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js" crossorigin></script>
<script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
```

2.jsx语法规则

- 创建虚拟DOM时,不要写引号
- 标签中要混入js表达式,要使用{}
- 标签中样式的类名要用className指定
- 标签中的内联样式要用style={{color: 'white'}},多个注意属性名转化为小驼峰
- 只能有一个根标签
- 标签必须闭合
- 关于标签首字母
  - 若首字母小写,那么React就会去找寻与之同名的HTML标签,若找见,直接转化为HTML同名元素,否则报错
  - 若首字母大写,那么React就会去找寻与之同名的HTML标签,若找见,那么就使用组件,否则报错