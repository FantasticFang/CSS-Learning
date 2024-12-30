## Position
#### Sticky
- position: sticky，常用于滚动的场景中
- 初始化时：containg block与static/relative的元素一致，为祖先元素中最近一级的块级元素content box，且top等属性不生效
- sticky属性生效：当滚动到最近一级的「滚动祖先元素」边界时，sticky属性生效，且只在该级祖先元素生效，不在更远的祖先元素中生效
- 当sticky生效，且竖向滚动时，top、bottom属性生效；同理，left、right属性在横向滚动时才生效
- top、bottom、left、right相对于最近一级的「滚动祖先元素」的content box生效