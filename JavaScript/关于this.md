####判断this

###一般情况下

1. 函数是否在new中调用（new绑定）？如果是的话this绑定的是新创建的对象。

	var bar = new foo()

2. 函数是否通过call、apply（显式绑定）或者硬绑定调用？如果是的话，this绑定的是指定的对象。
	
	var bar = foo.call(obj2)

3. 函数是否在某个上下文对象中调用（隐式绑定）？如果是的话，this绑定的是那个上下文对象。

	var var = obj1.foo()

4. 如果都不是的话，使用默认绑定。如果在严格模式下，就绑定到undefined，否则绑定到全局对象。

	var bar = foo()

###此外

ES6中的箭头函数并不会使用四条标准的绑定规则，而是根据当前的词法作用域来决定this，箭头函数会继承外层函数调用的this绑定（无论this绑定到什么）。这其实和ES6之前代码中的self = this机制一样。

