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