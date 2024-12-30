## Canvas
#### Canvas默认创建的坐标系
- 左上角为起点的笛卡尔坐标系
- (0,0) +----------------------------------> x
       |    (50, 50)
       |       *
       |              
       |              
       |                          
       |                         
       v y
- 其中x坐标系范围的最大值为[0, width]
- 其中y坐标系范围的最大值为[0, height]
- 超出canvas的范围的内容不会被渲染
- canvas渲染区域不存在滚动条

#### Canvas-2D API: fillText
- fillText(text, x, y)
- x为绘制text的第一个字的起点
- y为绘制text的baseline，需要注意，如果设置y=0的话，text根据baseline以上的部分，绘制到坐标系之外，会导致text不显示

#### Canvas-2D API: rotate
- rotate的传参为角度，但单位为「弧度(radians)」，而非「度(degree)」
- rotate的旋转中心为坐标轴起点（0，0）
- 如果想要改变rotate的旋转中心，则需要用「Canvas-2D API: translate」进行移动