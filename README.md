# 模块分析
> 一个JS模块分析打包工具

## 使用

```bash
# 打包并生成dist/index.html
$ npm run bundle
```

## JS代码的转换

1. @babel/parser 把JS文件转换成AST抽象语法树
2. @babel/traverse 遍历type为ImportDeclaration的AST获取import文件路径
3. @babel/core 将AST抽象语法树转换成浏览器支持的语法
