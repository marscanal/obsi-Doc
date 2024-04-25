```html
```<!DOCTYPE html>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  定义动画名
  animation-name: example;
  持续时间
  animation-duration: 4s;
  延迟执行，用负值，动画将开始播放，如同已播放 N 秒。
   animation-delay: 2s;
}

绑定关键帧
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
  也可以用百分比
  0%   {background-color: red;}
  25%  {background-color: yellow;}
  50%  {background-color: blue;}
  100% {background-color: green;}
  播放次数，也可以是无限，infinite
  animation-iteration-count: 3;
  播放方向，- `normal` - 动画正常播放（向前）。默认值
- `reverse` - 动画以反方向播放（向后）
- `alternate` - 动画先向前播放，然后向后
- `alternate-reverse` - 动画先向后播放，然后向前
  animation-direction: reverse;
  
}
</style>
</head>
<body>
	<div></div>
</body>
```