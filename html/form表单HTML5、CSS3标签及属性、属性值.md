form表单HTML5、CSS3标签及属性、属性值
form表单HTML标签、属性、属性值：
（单行文本输入框） （密码输入框） （单选框） （多选框） （提交按钮） （重置按钮） 或者按钮（空按钮） （下拉框选） （多行文本框）
（1） 是表单的标签，所有的需要写在form里面才能今 
进行提交； 
1：name=”” form中的name属性主要是对这个form进行标记； 
2：methood=”get/post” 其中 get/post 之间的区别： 
1. get是从服务器上获取数据，post是向服务器传送数据。 
2. get是把参数数据队列加到提交表单的ACTION属性所指的URL 
中，值和表单内各个字段一一对应，在URL中可以看到。post是通 
过HTTP post机制，将表单内各个字段与其内容放置在HTML 
HEADER内一起传送到ACTION属性所指的URL地址。用户看不到 
这个过程。 
3. 对于get方式，服务器端用Request.QueryString获取变量的值， 
对于post方式，服务器端用Request.Form获取提交的数据。 
4. get传送的数据量较小，不能大于2KB。post传送的数据量较大， 
一般被默认为不受限制。但理论上，IIS4中最大量为80KB，IIS5中 
为100KB。 
5. get安全性非常低，post安全性较高。但是执行效率却比Post方法 
好。 
3： action=”” action=url用来指定处理提交表单的格式.它可以是一个 
URL地址(提交给程式)或一个电子邮件地址. 
4：enctype=cdata指明用来把表单提交给服务器时(当method值为”post”) 
的互联网媒体形式.这个特性的缺省值是”application/x-www-form- 
urlencoded” 
5：target=”“指定提交的结果文档显示的位置： _blank ：在一个新的、 
无名浏览器窗口调入指定的文档； _self ：在指向这个目标的元素的相同 
的框架中调入文档； _parent ：把文档调入当前框的直接的 frameset 
框中；这个值在当前框没有父框时等价于_self； _top ：把文档调入原来 
的最顶部的浏览器窗口中(因此取消所有其它框架)；这个值等价于当前框 
没有你框时的_self. 
（2）type=”text”是定义表单里面的单行文本框；value=”“文本框里默认的文字；size=”“单行文本框的宽度；maxlength=”“单行文本框所能输入的字节； 
（3）type=”password” 定义密码框； 
（4）type=”radio” 单选勾选框； 
（5）type=”checkbox” 多选勾选框； 
（6）type=”submit” 提交按钮； 
（7）type=”reset” 重置按钮； 
（8）type=”button”或者 两种方式都可以实现空按钮； 
（9） 多行文本框，是一个双标签； 
（10） 


下拉菜单属性；

form表单css3属性、属性值：
1、表单字段集： 

功能：相当于一方框，在字段集中可以包含文本框包含其他元素，该元素 
用于对表单中元素进行分组，并在文档中区别出文本。fieldset元素可以嵌 
套，在其他内部可以再设置多个fieldset对象。 
2、字段集标题 

功能：legend元素可以再fieldset对象绘制的方框内插入一个标题。legend 
元素必须是fieldset内第一个元素。 
3、表单元素： 
（1）上传文件框 
文本域 
（2）图像域（图片按钮） 
form表单HTML5新增标签、属性、属性值：

1.email：专门用来输入email地址的文本框,如果该文本框中内容不是email地址格式的，则不允许提交。但它不检查email地址是否存在。提交时可以为空，除非加上了required属性。 
具有multiple属性，它允许在该文本框中输入一串以逗号分隔的email地址。 

2.url：专门用来输入URL地址的文本框。如果该文本框中内容不是URL地址格式的，则不允许提交。 
例：http://www.baidu.com”>

number 和 range 
number 类型是专门用来输入数字的，并且在提交时会检验是否为数字。number 类型有 max、min 和 step 属性。max 是允许的最大值，min 是允许的最小值，step 是间隔。设置了这些属性后，如果手动填入的数字不符合这些属性条件，将不能提交。 range 类型是一个数字滑动条。它与 number 类型功能类似，也有 max、min 和 step 属性，在 Opera 中，可以用左右方向键控制。range 类型自身没有一个明显的“数值”表示当前值，但可以使用 output 输出当前值。 

datetime 和 datetime-local 
datetime 类型是用来输入 UTC 日期和时间的文本框，而 datetime-local 类型是用来输入本地日期和时间的。它们与 date 类型的区别是后面多了一个时间框和“UTC”。 

month 和 weekmonth 类型是月份选择器，它的值为：年-月，如：2012-01；week 类型是周选择器，它的值为：年-W周数，如：2011-W02。 

search 
search 类型的是用来输入搜索关键词的文本框，它与 text 类型在功能都没有太大区别，只在外观上有细微的区别。在 Chrome 10 和 Safari 5 中，当用户输入内容时，输入框右侧会有一个“×”按钮，单击该按钮，将清空输入框内的内容，使用非常方便。 

7.color 
color 类型用来选取颜色，它提供了一个颜色选取器，值为 16 进制符号，如：#ff0000。目前只在 Opera 和 Blackberry 浏览器中支持。 

8.output元素： 定义不同类型的输出，如计算结果的输出，或脚本的输出。 
注：必须从属于某个表单。即，必须将它书写在表单内部，或对它添加form属性。 
0 
100+ 
= 



ML 5 不但新增加了表单元素、表单类型，还增加了一些表单属性，同时使用的话，能更好的提高率开发者的工作效率，同时也提高了用户的操作体验。 
1、自动验证 
1）、required 
可以应用在大多数输入元素上,在提交时如果元素内容为空白，则不允许提交，同时显示提示文字。 
2）、pattern 
将属性值设为某个格式的正则表达式，在提交时会检查其内容是否符合给定格式。 
例：

（3）placeholder属性：文本框处于未输入状态时文本框中显示的输入提示。

（4）autofocus属性：给文本框、选择框、或者按钮控件加上该属性，当打开页面时，该控件自动获得国标焦点，一个页面只能有一个。

（5） autocomplete 属性规定输入字段是否应该启用自动完成功能。属性值=on/off 
自动完成允许浏览器预测对字段的输入。当用户在字段开始键入时，浏览器基于之前键入过的值，应该显示出在字段中填写的选项。 
注释：autocomplete 属性适用于 ，以及下面的 类型：text, search, url, telephone, email, password, datepickers, range 以及 color。 
提示：在某些浏览器中，您可能需要手动启用自动完成功能。

HTML5增加了大量在提交时对表单及表单元素内容有效性验证的功能。

1、自动验证 
3）、 min、max、step：为包含数字或日期的 input 类型规定限定（约束） 
max: 最大值 
min: 最小值 
step: 数字间隔 
例： 
2、取消验证 
可以对form表单添加novalidate属性，即使form表单中的input添加了required，也将不进行验证

附：适用form表单的UI状态伪类选择器 


原文链接：https://blog.csdn.net/cainiaoqianduan/article/details/81591300