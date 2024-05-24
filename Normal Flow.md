## 正常流布局
#### 定义：
the way that webpage elements lay themselves out if you haven't changed their layout.
简单去理解就是按照相应格式化上下文规则去排序，从上到下；从左到右，排不下就换行
#### 具体布局：
- 块级元素：按块级格式化上下文排列
- 行内元素：按行内格式化上下文从左到右排列，排不下时，需要重新创建一个块级别行盒，之后在行盒中依然按IFC布局
- Float盒元素：左右方向上，根据float的值的属性，在left/right/inline-start/inline-end方向对齐containing box的边沿或者对齐到另一个float盒的边沿；上下方向上，float元素与行盒顶部对齐，如果有很多个float元素堆叠导致一行放不下，则会到下一行（为何将float元素写在这里，因为float依然属于正常流文档中的一部分，并不像绝对定位元素完全脱离文档流）