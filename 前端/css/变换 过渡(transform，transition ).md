下表列出了所有 2D 变换属性：

| 属性               | 描述                |
| ---------------- | ----------------- |
| transform        | 向元素应用 2D 或 3D 转换。 |
| transform-origin | 允许你改变被转换元素的位置。    |

## CSS 2D 转换方法

| 函数                              | 描述                       |
| ------------------------------- | ------------------------ |
| matrix(_n_,_n_,_n_,_n_,_n_,_n_) | 定义 2D 转换，使用六个值的矩阵。       |
| translate(_x_,_y_)              | 定义 2D 转换，沿着 X 和 Y 轴移动元素。 |
| translateX(_n_)                 | 定义 2D 转换，沿着 X 轴移动元素。     |
| translateY(_n_)                 | 定义 2D 转换，沿着 Y 轴移动元素。     |
| scale(_x_,_y_)                  | 定义 2D 缩放转换，改变元素的宽度和高度。   |
| scaleX(_n_)                     | 定义 2D 缩放转换，改变元素的宽度。      |
| scaleY(_n_)                     | 定义 2D 缩放转换，改变元素的高度。      |
| rotate(_angle_)                 | 定义 2D 旋转，在参数中规定角度。       |
| skew(_x-angle_,_y-angle_)       | 定义 2D 倾斜转换，沿着 X 和 Y 轴。   |
| skewX(_angle_)                  | 定义 2D 倾斜转换，沿着 X 轴。       |
| skewY(_angle_)                  | 定义 2D 倾斜转换，沿着 Y 轴。       |

```html
div {
	参数如下：matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(),translateY())
  transform: matrix(1, -0.3, 0, 1, 0, 0);
}

```

## CSS 3D 转换方法

通过 CSS `transform` 属性，您可以使用以下 3D 转换方法：

- `rotateX()`
- `rotateY()`
- `rotateZ()`z轴为二维里的y轴
```html
	#myDiv {
  transform: rotateX(150deg);
}
```

# CSS transition 属性
transition 属性是一个简写属性，用于设置四个过渡属性：
- transition-property
- transition-duration
- transition-timing-function
- transition-delay
注释：请始终设置 transition-duration 属性，否则时长为 0，就不会产生过渡效果。
```html
div {
  transition: width 2s linear 1s;
}
```