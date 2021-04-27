# 04 半透明边框

## `background-clip`属性
1. 在盒子本身有背景的情况下，如果直接设置边框为半透明颜色，实际上是不起作用的，因为`background-clip`属性的默认值是`border-box`，即背景会延申到边框盒子，这样一来即使边框是半透明的也看不出来了。
2. `background-clip`属性值可修改为`padding-box`,`content-box`等等，表示背景裁剪到哪个盒子的范围。
3. 利用这个特性可以实现半透明边框。
