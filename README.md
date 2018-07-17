# less-simple
## 这是一个简单快捷的less 我们称之 simple

//public font-size this want / 13.33<br />
//创建一个字体大小函数 默认小数点为2<br />
@fontSize:13.33;<br />
.font-size(@size,@digit:2){<br />
	font-size: round(@size / @fontSize,@digit) * @rem1;<br />
}<br />

//比如说 我们可以这样书写<br />
.font-size(100,4) => font-size:7.5018rem;<br />
.font-size(100) => font-size:7.50rem;<br />


//public height rem<br />
.height(@height){<br />
	height: @height * @rem1;<br />
}<br />

//比如说 我们可以这样书写<br />
.height(1) => height:1rem;<br />

//public line-height<br />
.line-height(@line-height){<br />
	line-height: @line-height * @rem1;<br />
}<br />

//比如说 我们可以这样书写<br />
.line-height(1) => line-height:1rem;<br />

//public height and line-height <br />
.heightAndLine(@height,@line-height:@height){<br />
	height: @height * @rem1;<br />
	line-height: @line-height * @rem1;<br />
}<br />

//比如说 我们可以这样书写<br />
.heightAndLine(1) => line-height:1rem;height:1rem;<br />
.heightAndLine(2,1) => line-height:1rem;height:2rem;<br />

//public text-center<br />
.text-center{<br />
	text-align: @center;<br />
}<br />

//比如说 我们可以这样书写<br />
.text-center => text-align: center;<br />


//public text-left<br />
.text-left{<br />
	text-align: @lf;<br />
}<br />
//public text-right<br />
.text-right{<br />
	text-align: @rg;<br />
}<br />

//public float left<br />
.float-lf{<br />
	float: @lf;<br />
}<br />

//public float right<br />
.float-rg{<br />
	float: @rg;<br />
}<br />


#后期会有更加多的函数参与进来
##欢迎大家多多动动大家的小手指 点击一下 Star
###有好的建议与要求可以可以提出 感激不尽
