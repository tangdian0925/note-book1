# 半圆笔记
## 预备课练习
### 1.在practice文件夹下文件文件夹new，在new文件夹下，新建new.txt 文件
 cd
 
mkdir -p prepare/practice/new

cd prepare/practice/new

touch new.txt
### 2.new.txt中增加文本，welcome to banyuan
echo "welcome to banyuan" > new.txt

### 3.在practice文件夹下新建newother文件夹，下面再建立一个sub文件夹，将new.txt 复制到sub文件夹下
cd

cd prepare/practice

mkdir -p newother/sub

cp new/new.txt newother/sub
### 4将new文件夹下new.txt重新命名为 new1.txt
cd

cd prepare/practice/new

mv new.txt new1.txt
### 5.将sub文件夹整个移动到 practice 文件夹下，命名为new2

cd

cd prepare/practice

mv newother/sub new2
### 6.将practice下的new开头的文件夹都删除掉
cd

cd prepare/practice
rm new.txt
rm new2
 
## markdown的运用
# 一级标题
#加空格+一级标题
## 二级标题 
##加空格+二级标题
。。。。。

 正文
## 字体
### **加粗**
要加粗的文字左右分别用两个*号包起来

### *斜体*
要倾斜的文字左右分别用一个*号包起来

### ***斜体加粗***
要倾斜和加粗的文字左右分别用三个*号包起来

## 分割线
三个或者三个以上的 - 或者 * 都可以。

## 图片
### 语法
![图片alt](图片地址''图片title'')

图片alt就是显示在图片下面的文字，相当于对图片内容的解释。

图片title是图片的标题，当鼠标移到图片上时显示的内容。title可加可不加

## 超链接
[超链接名](超链接地址 "超链接title")

title可加可不加

## 列表
### 无序列表
无序列表用 - + * 任何一种都可以

* 你好
* 你好
* 你好

### 有序列表
数字加点

1.你好

2.你好

3.你好

### 列表嵌套
上一级和下一级之间敲三个空格即可

* 你好
   * 你好

### 表格
表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

第二行分割表头和内容。
- 有一个就行，为了对齐，多加了几个
文字默认居左
-两边加：表示文字居中
-右边加：表示文字居右
注：原生的语法两边都要用 | 包起来。

### 代码
单行代码：代码之间分别用一个反引号包起来

代码块：代码之间分别用三个反引号包起来，且两边的反引号单独占一行

### 流程图
```flow
st=>start: 开始
op=>operation: My Operation
cond=>condition: Yes or No?
e=>end
st->op->cond
cond(yes)->e
cond(no)->op
&```

课后练习
继续学习mac快捷键
继续提升打字速度
继续学习鸟叔教程