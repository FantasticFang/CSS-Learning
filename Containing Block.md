## Containing Block
#### 定义
The size and position of an element are often impacted by its containing block.
Most often, the containing block is the content area of an element's nearest block-level ancestor, but this is not always the case.
Containing Block实际上定义了元素的大小和位置的依据
#### 为何Containing Block很重要？
- 如上述定义中所说，Containing Block会影响元素的大小和位置
- 当元素的大小/位置相关属性为百分比单位时，就需要根据Containing Block的宽度/高度来计算。元素的width、margin、padding、left、right根据Containing Block的宽度来计算；元素的height、top、bottom根据Containing Block的高度来计算
#### 不同情况下对应的Containing Block
- root element(html)对应的Containing Block：viewport
- position为static、relative、sticky时对应的Containing Block：祖先元素中，最近一级的块元素（block container）的Content Box；祖先元素中，最近一级创建了格式化上下文的容器（table container、flex container、grid container、block container）的content box
- position为sticky时，初始化时的Containing Block与static和relative一致，这时候top、left等属性也是不生效的；当滚动使sticky属性生效时，top、left是相对于最近的一级可滚动的祖先元素的Content Box来计算
- position为absolute时对应的Containing Block：祖先元素中，最近一级position属性为非static的元素的padding box
- position为fixed时对应的Containing Block：viewport
- Note: 当postion为fixed或者absolute时，containing block也受transform、fitler(?)、will-change(?)、contain(?)、container-type(?)、backdrop-filter(?)任意一种的影响