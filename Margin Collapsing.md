## Margin Collapsing
#### 发生条件：
- 块级元素
- 相邻的兄弟节点中
- 父级组件与子组件之间无内容，eg: there is no border, padding, inline part, block formattingcontext, or clearance
- 空元素，margin top & margin bottom会发生collapse
- Margin Collapsing可能发生于以上的组合条件
- Margin Collapsing不会发生在浮动或者绝对定位元素中
- 及时父元素的margin设置为0，也不能避免Margin Collapsing
- 如果发生Margin Collapsing的一方margin为负值，一方为正值，那么最后的margin值为两者之和，如果均为负值，那margin为最小的负值数值
- 只有竖直方向会发生Margin Collapsing
- 处于flex/grid布局中的元素不会发生Margin Collapsing
#### 避免Margin Collapsing方法
- 对于嵌套元素，那么只需要设置父级元素的border/padding/clearance
- 对于相邻元素，那么我们可以接受Margin Collapsing的设计，因为理论上的UI设计会保持同级别元素的margin一致；亦或用flex/grid布局
