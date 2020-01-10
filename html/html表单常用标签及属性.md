# [form(表单)标签常用标签及属性](https://www.cnblogs.com/1500418882qqcom/p/9605503.html)

## 1.表单标签语法：

 <form method="传送方式" action="服务器文件"></form>

 (1)<form>标签成对出现,

 (2)两种数据传送方式（get/post）

 

 

## 2.文本框,密码框：

###  语法：

  <form>

  <input type="text/password" name="名称" value="文本">

  </form>

（1）type="text"时，输入框为文本框

（2）type="password"时，输入框为密码框

（3）name，命名文本框

（4）value，文本框输入的默认值

例：

<form>

 姓名:<input type="text">

 密码:<input type="password">

</form>

 

 

## 3.多行文本：

 语法：

<form>

 <textarea rows="行数" cols="列数"></textarea>

</form>

例：

<form>

 <textarea rows="10" cols="10"></textarea>

</form>

 

 

## 4.单选框,多选框

语法：

<form>

 <input type="radio/checkbox" value="值" name="名称">

</form>

type=“radio”时，输入框为单选框

type=“checkbox”时，输入框为多选框

例：

<form>

 <input type="radio" value="' name="">是

 <input type="radio" value="" name="">否

</form>

<form>

 <input type="checkbox" value="" name="">1

 <input type="checkbox" value="" name="">2

 <input type="checkbox" value="" name="">3

</form>

 

 

## 5.下拉列表框：

语法：

<form>

 <select>

   <option value="值"></option>

   <option value="值"></option>

   <option value="值"></option>

 </select>

</form>

 

 

## 6.下拉列表多选框：

语法：

<form>

 <select **multiple**>

   <option></option>

   <option></option>

 <select>

</form>

 

 

## 7.普通，提交，重置按钮：

语法：

<form>

 <input type="button" value="普通按钮">

 <input type="submit" value="提交按钮">

 <input type="reset" value="重置按钮">

</form>

