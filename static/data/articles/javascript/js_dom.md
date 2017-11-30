## node 类型
- 1 -> element
- 2 -> attribute
- 3 -> text

## document 类型
- 表示整个HTML页面
- document对象是window对象的一个属性
- nodeType = 9
- attribute
	- URL: 完整的URL
	- domain: 域名 
		- 可设置，只能往更松散的方向设置
		- 只能设置同一个域的域名
	- referrer: 来源页面


## element 类型
- nodeType = 1
- nodeName = tagName
- nodeValue = null
- parentNode
- HTMLElement继承Element, 并添加了一些属性
	- attribute
 	- getAttribute()
 	- setAttribute()
 	- removeAttribute()
 	
- 分清属性(property)和特性(attribute)
- 属性是object的property
- 特性是HTML元素的attribute
- 可以通过obejct.property set/get 存在的property，自定义的不可以，只能通过getAttribute()/setAttribute()
- 还是建议通过设置property来改变attribute
- HTML5标准，自定义attribute应该用'data-'


## text 类型
- nodeType = 3
- nodeName = '#text'
- nodeValue
- parentNode -> element
- childNode -> not support

- document.createTextNode()
- element.normalize(): 合并文本节点
- splitText(): 分割文本节点

## comment 类型
- nodeType = 8
- nodeName = '#comment'
- nodeValue -> 注释的内容
- parentNode -> document/element
- childNode -> not support
- 与text类型继承相同的基类

## CDATASection 类型(XML only)
- nodeType = 4
- nodeName = '#cdata-section'
- nodeValue -> content

## documentType 类型

## documentFragment 类型

## attr 类型 (不建议直接操作)
- nodeType = 11
- nodeName = attr name
- nodeValue = attr value
- parentNode = null
- childNode -> not support
- properties:
    - .name = nodeName 
    - .value = nodeValue
    - .specified = boolean


- document.querySelector('#div');
- document.querySelectorAll('.div');


## HTML5 new 
- document.getEelementSByClassName()
- classList
    - classList.add()
    - classList.contains()
    - classList.remove()
    - classList.toggle()


















