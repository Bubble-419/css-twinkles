# 06 CSS翻转效果
## 前置知识
1. CSS 3D属性
  **`perspective`**
  定义3d元素距离视图的距离，当定义该属性时，其子元素会获得透视效果。
  **`transform`**
  一些3d旋转方法。
## 思路：
1. 父盒子声明`perspective`，开启3d空间。子盒子声明`transform-style: preserve-3d;`，保留3d空间。
2. 将背面盒子翻转180°，同时声明`backface-visibility: hidden;`隐藏3d背面。
3. 声明hover或click时翻转。
