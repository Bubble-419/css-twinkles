# 05 Button-hover-effects

## 涉及知识

1. **outline**

   声明元素的轮廓，通常用于表单元素、链接等，与`border`的区别是不会占用空间，即不会影响盒子模型。

2. [**svg**](https://developer.mozilla.org/zh-CN/docs/Web/SVG)

   - svg元素和svg属性

     元素应用于矢量图形的布局、结构、绘制

     属性用于控制元素的呈现

   - 常见元素：`rect`, `circle`, `ellipse`，都可以设置一些基本属性：`rect`的x，y坐标和宽高，两个圆的cx，cy（圆心）坐标和rx半径等

   - stroke系列属性

     `stroke`属性定义了给定图形元素的外轮廓的颜色。

     `stroke-dasharray`属性用一个数组描绘虚线边框的短划线和缺口值。如果提供了奇数个值，则这个值的数列重复一次，从而变成偶数个值。

     `stroke-offset`属性定义了第一条虚线距离开始路径的值。

3. CSS3动画

   - `@keyframes`规则，可以定义`from`和`to`的效果，也可以直接定义`to`

     ```css
     @keyframes example {
       from {background-color: red;}
       to {background-color: yellow;}
     }
     ```

   - [`animation`属性](https://developer.mozilla.org/zh-CN/docs/Web/CSS/animation)

## 实现思路

1. 按钮1

   >  按钮1的特效由两部分组成：
   >
   > 1. hover前边框半透明，hover时边框透明度提高且具备内阴影
   >
   > 2. hover时有边框往外移动逐渐消失的特效，利用outline透明度过渡为0实现

2. 按钮2

   > 伪元素的移动

3. 按钮3

   > 通过颜色和阴影的变换营造突起和按下感

4. 按钮4

   > 利用svg的stroke系列属性和hover伪类选择器

5. 按钮5

   > 利用svg和CSS3动画

6. 按钮4和5相比，动画特效显得不太自然