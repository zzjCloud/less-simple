# less-simple
## 这是一个简单快捷的less 我们称之 simple

//public font-size this want / 13.33<br />
@fontSize:13.33;<br />
.font-size(@size,@digit:2){<br />
	font-size: round(@size / @fontSize,@digit) * @rem1;<br />
}<br />

//public padding and margin this size want / 26.66 <br />
@distance:26.66;<br />
.proportions(@name,@proportionTop,@proportionRight:@proportionTop,@proportionBottom:@proportionTop,@proportionLeft:@proportionRight,@digit:2){<br />
	@{name}:round(@proportionTop / @distance,@digit) * @rem1 round(@proportionRight / @distance,@digit) * @rem1 round(@proportionBottom / @distance,@digit) * @rem1 round(@proportionLeft / @distance,@digit) * @rem1<br />
}<br />



//public height rem<br />
.height(@height){<br />
	height: @height * @rem1;<br />
}<br />

//public line-height<br />
.line-height(@line-height){<br />
	line-height: @line-height * @rem1;<br />
}<br />

//public height and line-height <br />
.heightAndLine(@height,@line-height:@height){<br />
	height: @height * @rem1;<br />
	line-height: @line-height * @rem1;<br />
}<br />

//public text-center<br />
.text-center{<br />
	text-align: @center;<br />
}<br />
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
