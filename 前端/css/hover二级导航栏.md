1.父级元素：相对定位
2.隐藏元素：display: none;
3.hover注意 [[选择器]]
```html
<div class="item-tittle">
	<h3>
		<a href="#" class=''>参考书</a>
	</h3>
	<div class="item-list">
		<h4>details</h4>
		<h4>details</h4>
		<h4>details</h4>
	</div>
 </div>
```

```js
.item-tittle {
  width: 200px;
  height: 500px;
  父级元素：相对定位
  position: relative;
}

.item-list {
  position: absolute;
  left: 200px;
  top: 0px;
  隐藏元素
  display: none;
}
hover注意选择器，+相邻兄弟
.item-tittle h3:hover + .item-list {
  display: inline-block;
}
```