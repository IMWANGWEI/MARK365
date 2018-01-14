####CSS Hack
一般来说就是针对不同的浏览器写不同的CSS，那就是CSS Hack

IE浏览器Hack一般又分为三种，条件Hack、属性级Hack、选择符Hack

	//1、条件Hack
	<!--[if IE]>
	<style>
	.test{color: red}
	</style>
	<![endif]-->

	//2、属性Hack
	.test{
		color: #0909; /* For IE8+ */
		color: #f00; /* For IE7 and earlier */
		_color: #ff0; /* For IE6 and earlier */
	}

	//3、选择符Hack
	html.test{color:#090;} /* For IE6 and earlier */
	html.test{color:#ffo;} /* For IE7 */

具体参考[这里](http://blog.csdn.net/freshlover/article/details/12132801 "Hack")或者[这里](https://www.duitang.com/static/csshack.html)