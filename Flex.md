## flex
#### 定义：
- display: flex，定义了一个元素是弹性容器（flex container），其子元素为弹性子元素（flex item），弹性容器会占满可用宽度（所谓可用宽度，定义宽度/未定义宽度时为100%）（百分比单位由该容器的containing block决定）
- display: inline-flex，与display: flex定义类似，只不过该容器以行内元素参与排列，且容器宽度不会自动膨胀至100%

#### 布局策略：
- flex布局，定义了一个主轴（main axis），以及一个副轴（cross axis）
- 主轴默认为水平方向，副轴默认为垂直方向（通过flex-direction可自定义）
- 