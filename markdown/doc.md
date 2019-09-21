### 一、标题
- 根据#的个数，一个#表示一级，类推可以到六级(类比HTML中h1~h6)

### 二、字体
- 加粗：两个\*号: **这是加粗的内容**
- 斜体：一个\*号: *这是斜体*
- 加粗和斜体：3个\*号: ***这是加粗和斜体内容***
- 删除线：两个\~: ~~这是删除线~~

### 三、引用
- 用符号\>，也可以多个\>符号
  > 这是引用的内容
  > 这是引用的内容
  >
  > > 这是引用的内容

### 四、分割线
- 三个或三个以上的*或者-号,效果一样
  ***
  ----

### 五、超链接
- 语法：[超链接](超链接地址 "title")，title可以没有，下面两种方式等效
  1. [百度](http://www.baidu.com "百度")
  2. <a href="http://www.baidu.com" target="_blank" title="百度">百度</a>
  3. 图片显示语法：\!\[说明\](地址 "title")，注意有个感叹号

### 六、列表
- 无序列表：+、-、*都可以
 * 这是列表
    * 嵌套列表（与上一级列表前相差三个空格）
       * 嵌套列表
  - 这是列表
  + 这是列表
- 有序列表：数字加"**.**"，"**.**"和后面的内容要有空格
 1. 有序
     1. 子序1
     2. 子序2（一旦子序1的数字被确定，子序2前的序号就被确定了，即便这儿写成3，显示的也是2）

### 七、表格
- 语法：
   - **-:**表示内容和标题栏居右对齐
   - **:-**表示居左对齐
   - **:-:**表示居中对齐
  \|表头|表头|
  |---|---|
  |内容|内容|
  例如：
  |姓名|技能|排行|
  |:--:|:--:|:--:|
  |刘备|哭|大哥|
  |关羽|打|二哥|
  |张飞|骂|三弟|

### 八、代码
- 语法：单行代码之间用反引号引起来
  `System.out.println("hello world");`
- 代码块：用三个反引号，反引号要独占一行
 ```
  def sum():
      sum = 0
      for i in range(1, 101):
          sum += i
      return sum
 ```

### 九、为文档添加目录

- 当文档内容过多时，需要增加一个目录来进行业内跳转

  使用语法: 

  ```
  <!--TOC-->
     目录内容
  <!--/TOC-->
  ```
  
  注意，[TOC]要单独占一行


### 十、页内任意跳转

- 使用语法：`[描述](#目录)`，这儿表示跳转到目录，#后面接的就是跳转到的标题(具有h1-h6的就是标题)，#后面也可以跟id，例如<a id="xxxx"></a>，那么就可一跳转到该链接处