# cssTwinkle
some html+css small projects, just for practicing. I hope I can persist, and have more thoughts.

## 001 parallexScrolling 视差滚动
### [moonlight #tag: js实现/渐变效果](https://github.com/Bubble-419/cssTwinkle/tree/main/01parallaxScrolling/01moonlight)
#### 思路：
1. 制作视差滚动特效时，网页元素可以看作图片编辑中的“图层”来处理，每一个图层有不同的移动速度，从而形成了不一样的视觉效果。这个项目的实现重点就在于**给“图层”即元素，创造不同的移动速度**。

2. 从图片的排版可以自然而然地联想到“子绝父相”的定位布局，要注意布局时可以使用`object-fit: cover;`使得图片自适应容器。

3. 使用一个`::before`选择器配合`linear-gradient()`来创造渐变效果，使用`::after`选择器配合`mix-blend-mode`属性来创造颜色混合效果。 
    *linear-gradient(direction, color-stop1, color-stop2, ...). color-stop用于指定渐变的起止色*
    *mix-blend-mode:类似ps中的颜色混合模式*
    
4. js部分：获取window对象的scroll值，乘以不同的倍数赋给元素的top/left值，产生移动速度差，注意正负值。

## 002 字体发光特效
### [font-awesome #图标字体+svg](https://github.com/Bubble-419/cssTwinkle/tree/main/02font-awesome)
#### 思路：
1. 利用伪元素选择器制作外发光，利用shadow制作内发光
2. 过渡动画和transform变换是锦上添花
3. 具体思路见注释
