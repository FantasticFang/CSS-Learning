## BFC
#### 定义：
块级格式化上下文，决定了块级元素的排列方式，从上到下排列
#### 创建BFC的方法
- 浮动元素
- 绝对定位元素
- 非块级别但能包含块级元素的容器（例如：display: inline-block、table-cell）
- 能包含块级元素的块级容器(块级容器，且overflow不等于visible，因为如果是visible相当于这个容器在布局中已经可以被忽略了)