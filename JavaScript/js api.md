###js各种方法了解一下

####Array 对象

Array 对象用于在单个的变量中存储多个值。

####创建 Array 对象的语法：

	new Array();
	new Array(size);
	new Array(element0, element1, ..., elementn);

#####参数

参数 size 是期望的数组元素个数。返回的数组，length 字段将被设为 size 的值。

参数 element ..., elementn 是参数列表。当使用这些参数来调用构造函数 Array() 时，新创建的数组的元素就会被初始化为这些值。它的 length 字段也会被设置为参数的个数。

#####返回值

返回新创建并被初始化了的数组。

如果调用构造函数 Array() 时没有使用参数，那么返回的数组为空，length 字段为 0。

当调用构造函数时只传递给它一个数字参数，该构造函数将返回具有指定个数、元素为 undefined 的数组。

当其他参数调用 Array() 时，该构造函数将用参数指定的值初始化数组。

当把构造函数作为函数调用，不使用 new 运算符时，它的行为与使用 new 运算符调用它时的行为完全一样。

#####Array 对象属性

	属性	                    描述
	
	constructor 	返回对创建此对象的数组函数的引用。
	
	length 	        设置或返回数组中元素的数目。
	
	prototype 	    使您有能力向对象添加属性和方法。

#####Array 对象方法
   
	方法 	                		描述
	concat() 	 		连接两个或更多的数组，并返回结果。
	join() 	     		把数组的所有元素放入一个字符串。元素通过指定的分隔符进行分隔。
	pop() 	     		删除并返回数组的最后一个元素
	push() 	     		向数组的末尾添加一个或更多元素，并返回新的长度。
	reverse() 	 		颠倒数组中元素的顺序。
	shift() 	 		删除并返回数组的第一个元素
	slice()      		从某个已有的数组返回选定的元素
	sort() 	     		对数组的元素进行排序
	splice() 	 		删除元素，并向数组添加新元素。
	toSource() 	 		返回该对象的源代码。
	toString() 	        把数组转换为字符串，并返回结果。
	toLocaleString() 	把数组转换为本地数组，并返回结果。
	unshift() 	        向数组的开头添加一个或更多元素，并返回新的长度。
	valueOf() 	        返回数组对象的原始值

####String

String 对象用于处理文本（字符串）。

#####创建 String 对象的语法：

	new String(s);
	String(s);

#####参数

参数 s 是要存储在 String 对象中或转换成原始字符串的值。

#####返回值

当 String() 和运算符 new 一起作为构造函数使用时，它返回一个新创建的 String 对象，存放的是字符串 s 或 s 的字符串表示。

当不用 new 运算符调用 String() 时，它只把 s 转换成原始的字符串，并返回转换后的值。

#####String 对象属性
	
	属性 				描述
	constructor 	对创建该对象的函数的引用
	length 	        字符串的长度
	prototype 	    允许您向对象添加属性和方法

#####String 对象方法

	方法 	                         描述
	anchor() 				创建 HTML 锚。
	big() 					用大号字体显示字符串。
	blink() 				显示闪动字符串。
	bold() 					使用粗体显示字符串。
	charAt() 				返回在指定位置的字符。
	charCodeAt() 			返回在指定的位置的字符的 Unicode 编码。
	concat() 				连接字符串。
	fixed() 				以打字机文本显示字符串。
	fontcolor() 			使用指定的颜色来显示字符串。
	fontsize() 				使用指定的尺寸来显示字符串。
	fromCharCode() 			从字符编码创建一个字符串。
	indexOf() 				检索字符串。
	italics() 				使用斜体显示字符串。
	lastIndexOf() 			从后向前搜索字符串。
	link() 					将字符串显示为链接。
	localeCompare() 		用本地特定的顺序来比较两个字符串。
	match() 	        	找到一个或多个正则表达式的匹配。
	replace() 				替换与正则表达式匹配的子串。
	search() 				检索与正则表达式相匹配的值。
	slice() 				提取字符串的片断，并在新的字符串中返回被提取的部分。	
	small() 				使用小字号来显示字符串。
	split() 				把字符串分割为字符串数组。
	strike() 				使用删除线来显示字符串。
	sub() 					把字符串显示为下标。
	substr() 				从起始索引号提取字符串中指定数目的字符。
	substring() 			提取字符串中两个指定的索引号之间的字符。
	sup() 					把字符串显示为上标。
	toLocaleLowerCase() 	把字符串转换为小写。
	toLocaleUpperCase() 	把字符串转换为大写。
	toLowerCase() 			把字符串转换为小写。
	toUpperCase() 			把字符串转换为大写。
	toSource() 				代表对象的源代码。
	toString() 				返回字符串。
	valueOf() 				返回某个字符串对象的原始值。

####Math 对象

Math 对象用于执行数学任务。

#####使用 Math 的属性和方法的语法：

	var pi_value=Math.PI;
	var sqrt_value=Math.sqrt(15);

注释：Math 对象并不像 Date 和 String 那样是对象的类，因此没有构造函数 Math()，像 Math.sin() 这样的函数只是函数，不是某个对象的方法。您无需创建它，通过把 Math 作为对象使用就可以调用其所有属性和方法。

#####Math 对象属性

	属性 						描述
	E 			返回算术常量 e，即自然对数的底数（约等于2.718）。
	LN2 		返回 2 的自然对数（约等于0.693）。
	LN10 		返回 10 的自然对数（约等于2.302）。
	LOG2E 		返回以 2 为底的 e 的对数（约等于 1.414）。
	LOG10E 		返回以 10 为底的 e 的对数（约等于0.434）。
	PI 			返回圆周率（约等于3.14159）。
	SQRT1_2 	返回返回 2 的平方根的倒数（约等于 0.707）。
	SQRT2 		返回 2 的平方根（约等于 1.414）。

#####Math 对象方法

	方法 				描述
	abs(x) 		返回数的绝对值。
	acos(x) 	返回数的反余弦值。
	asin(x) 	返回数的反正弦值。
	atan(x) 	以介于 -PI/2 与 PI/2 弧度之间的数值来返回 x 的反正切值。
	atan2(y,x) 	返回从 x 轴到点 (x,y) 的角度（介于 -PI/2 与 PI/2 弧度之间）。
	ceil(x) 	对数进行上舍入。
	cos(x) 		返回数的余弦。
	exp(x) 		返回 e 的指数。
	floor(x) 	对数进行下舍入。
	log(x) 		返回数的自然对数（底为e）。
	max(x,y) 	返回 x 和 y 中的最高值。
	min(x,y) 	返回 x 和 y 中的最低值。
	pow(x,y) 	返回 x 的 y 次幂。
	random() 	返回 0 ~ 1 之间的随机数。
	round(x) 	把数四舍五入为最接近的整数。
	sin(x) 		返回数的正弦。
	sqrt(x) 	返回数的平方根。
	tan(x) 		返回角的正切。
	toSource() 	返回该对象的源代码。
	valueOf() 	返回 Math 对象的原始值。

####Boolean 对象

Boolean 对象表示两个值："true" 或 "false"。

#####创建 Boolean 对象的语法：

	new Boolean(value);	//构造函数
	Boolean(value);		//转换函数

#####参数

参数 value 由布尔对象存放的值或者要转换成布尔值的值。

#####返回值

当作为一个构造函数（带有运算符 new）调用时，Boolean() 将把它的参数转换成一个布尔值，并且返回一个包含该值的 Boolean 对象。

如果作为一个函数（不带有运算符 new）调用时，Boolean() 只将把它的参数转换成一个原始的布尔值，并且返回这个值。

注释：如果省略 value 参数，或者设置为 0、-0、null、""、false、undefined 或 NaN，则该对象设置为 false。否则设置为 true（即使 value 参数是字符串 "false"）。

#####Boolean 对象属性

	属性 	                      描述
	constructor 	返回对创建此对象的 Boolean 函数的引用
	prototype 		使您有能力向对象添加属性和方法。

#####Boolean 对象方法

	方法 							描述
	toSource() 	返回该对象的源代码。
	toString() 	把逻辑值转换为字符串，并返回结果。
	valueOf() 	返回 Boolean 对象的原始值。

#####Boolean 对象描述

在 JavaScript 中，布尔值是一种基本的数据类型。Boolean 对象是一个将布尔值打包的布尔对象。Boolean 对象主要用于提供将布尔值转换成字符串的 toString() 方法。

当调用 toString() 方法将布尔值转换成字符串时（通常是由 JavaScript 隐式地调用），JavaScript 会内在地将这个布尔值转换成一个临时的 Boolean 对象，然后调用这个对象的 toString() 方法。

####Number 对象

Number 对象是原始数值的包装对象。

#####创建 Number 对象的语法：

	var myNum=new Number(value);
	var myNum=Number(value);

#####参数

参数 value 是要创建的 Number 对象的数值，或是要转换成数字的值。

#####返回值

当 Number() 和运算符 new 一起作为构造函数使用时，它返回一个新创建的 Number 对象。如果不用 new 运算符，把 Number() 作为一个函数来调用，它将把自己的参数转换成一个原始的数值，并且返回这个值（如果转换失败，则返回 NaN）。

#####Number 对象属性

	属性 						描述
	constructor 		返回对创建此对象的 Number 函数的引用。
	MAX_VALUE 			可表示的最大的数。
	MIN_VALUE 			可表示的最小的数。
	NaN 				非数字值。
	NEGATIVE_INFINITY 	负无穷大，溢出时返回该值。
	POSITIVE_INFINITY 	正无穷大，溢出时返回该值。
	prototype 			使您有能力向对象添加属性和方法。

#####Number 对象方法

	方法 					描述
	toString 		把数字转换为字符串，使用指定的基数。
	toLocaleString 	把数字转换为字符串，使用本地数字格式顺序。
	toFixed 		把数字转换为字符串，结果的小数点后有指定位数的数字。
	toExponential 	把对象的值转换为指数计数法。
	toPrecision 	把数字格式化为指定的长度。
	valueOf 		返回一个 Number 对象的基本数字值。

#####Number 对象描述

在 JavaScript 中，数字是一种基本的数据类型。JavaScript 还支持 Number 对象，该对象是原始数值的包装对象。在必要时，JavaScript 会自动地在原始数据和对象之间转换。在 JavaScript 1.1 中，可以用构造函数 Number() 明确地创建一个 Number 对象，尽管这样做并没有什么必要。

构造函数 Number() 可以不与运算符 new 一起使用，而直接作为转化函数来使用。以这种方式调用 Number() 时，它会把自己的参数转化成一个数字，然后返回转换后的原始数值（或 NaN）。

构造函数通常还用作 5 个有用的数字常量的占位符，这 5 个有用的数字常量分别是可表示的最大数、可表示的最小数、正无穷大、负无穷大和特殊的 NaN 值。 注意，这些值是构造函数 Number() 自身的属性，而不是单独的某个 Number 对象的属性。

比如这样使用属性 MAX_VALUE 是正确的：

	var big = Number.MAX_VALUE

但是这样是错误的：

	var n= new Number(2);
	var big = n.MAX_VALUE

作为比较，我们看一下 toString() 和 Number 对象的其他方法，它们是每个 Number 对象的方法，而不是 Number() 构造函数的方法。前面提到过，在必要时，JavaScript 会自动地把原始数值转化成 Number 对象，调用 Number 方法的既可以是 Number 对象，也可以是原始数字值。

	var n = 123;
	var binary_value = n.toString(2);

####Date 对象

Date 对象用于处理日期和时间。

#####创建 Date 对象的语法：

	var myDate=new Date()

注释：Date 对象会自动把当前日期和时间保存为其初始值。

#####Date 对象属性

	属性 				描述
	constructor 	返回对创建此对象的 Date 函数的引用。
	prototype 		使您有能力向对象添加属性和方法。

#####Date 对象方法

	方法 								描述
	Date() 					返回当日的日期和时间。
	getDate() 				从 Date 对象返回一个月中的某一天 (1 ~ 31)。
	getDay() 				从 Date 对象返回一周中的某一天 (0 ~ 6)。
	getMonth() 				从 Date 对象返回月份 (0 ~ 11)。
	getFullYear() 			从 Date 对象以四位数字返回年份。
	getYear() 				请使用 getFullYear() 方法代替。
	getHours() 				返回 Date 对象的小时 (0 ~ 23)。
	getMinutes() 			返回 Date 对象的分钟 (0 ~ 59)。
	getSeconds() 			返回 Date 对象的秒数 (0 ~ 59)。
	getMilliseconds() 		返回 Date 对象的毫秒(0 ~ 999)。
	getTime() 				返回 1970 年 1 月 1 日至今的毫秒数。
	getTimezoneOffset() 	返回本地时间与格林威治标准时间 (GMT) 的分钟差。
	getUTCDate() 			根据世界时从 Date 对象返回月中的一天 (1 ~ 31)。
	getUTCDay() 			根据世界时从 Date 对象返回周中的一天 (0 ~ 6)。
	getUTCMonth() 			根据世界时从 Date 对象返回月份 (0 ~ 11)。
	getUTCFullYear() 		根据世界时从 Date 对象返回四位数的年份。
	getUTCHours() 			根据世界时返回 Date 对象的小时 (0 ~ 23)。
	getUTCMinutes() 		根据世界时返回 Date 对象的分钟 (0 ~ 59)。
	getUTCSeconds() 		根据世界时返回 Date 对象的秒钟 (0 ~ 59)。
	getUTCMilliseconds() 	根据世界时返回 Date 对象的毫秒(0 ~ 999)。
	parse() 				返回1970年1月1日午夜到指定日期（字符串）的毫秒数。
	setDate() 				设置 Date 对象中月的某一天 (1 ~ 31)。
	setMonth() 				设置 Date 对象中月份 (0 ~ 11)。
	setFullYear() 			设置 Date 对象中的年份（四位数字）。
	setYear() 				请使用 setFullYear() 方法代替。
	setHours() 				设置 Date 对象中的小时 (0 ~ 23)。
	setMinutes() 			设置 Date 对象中的分钟 (0 ~ 59)。
	setSeconds() 			设置 Date 对象中的秒钟 (0 ~ 59)。
	setMilliseconds() 		设置 Date 对象中的毫秒 (0 ~ 999)。
	setTime() 				以毫秒设置 Date 对象。
	setUTCDate() 			根据世界时设置 Date 对象中月份的一天 (1 ~ 31)。
	setUTCMonth() 			根据世界时设置 Date 对象中的月份 (0 ~ 11)。
	setUTCFullYear() 		根据世界时设置 Date 对象中的年份（四位数字）。
	setUTCHours() 			根据世界时设置 Date 对象中的小时 (0 ~ 23)。
	setUTCMinutes() 		根据世界时设置 Date 对象中的分钟 (0 ~ 59)。
	setUTCSeconds() 		根据世界时设置 Date 对象中的秒钟 (0 ~ 59)。
	setUTCMilliseconds() 	根据世界时设置 Date 对象中的毫秒 (0 ~ 999)。
	toSource() 				返回该对象的源代码。
	toString() 				把 Date 对象转换为字符串。
	toTimeString() 			把 Date 对象的时间部分转换为字符串。
	toDateString() 			把 Date 对象的日期部分转换为字符串。
	toGMTString() 			请使用 toUTCString() 方法代替。
	toUTCString() 			根据世界时，把 Date 对象转换为字符串。
	toLocaleString() 		根据本地时间格式，把 Date 对象转换为字符串。
	toLocaleTimeString() 	根据本地时间格式，把 Date 对象的时间部分转换为字符串。
	toLocaleDateString() 	根据本地时间格式，把 Date 对象的日期部分转换为字符串。
	UTC() 					根据世界时返回 1970 年 1 月 1 日 到指定日期的毫秒数。
	valueOf() 				返回 Date 对象的原始值。