---
title: Python Tips
date: 2016-12-25 19:28:32
tags:
---

##	range
```python	
range(m,n)	#产生等差数列，序列开始于m，重复加1，直到n之前的n-1。
range(n)	#等价于range(0,n)
range(m,n,s)	#步长s：step value，变步长的整数序列。
```





## encode&decode
1.	string

		In computing, a string is a particular series of letters, numbers, symbols, or spaces, for example a word or phrase that you want to search for in a document.

2.	byte

		In computing, a byte is a unit of storage approximately equivalent to one printed character.
3.	string类型才可以encode('utf8')
4.	byte类型才可以decode('utf8')
5.	python3中汉字就是unicode编码

		print(print('a'=='\u0061')
		True

## python文档资源

*	dir	列出对象中可用属性列表

		import sys
		dir(sys)

*	查看内置对象类型提供的属性

		dir([])	#查看列表属性
		dir('')	#查看字符串属性


*	查看用户定义的文档字符串（三重引号块字符）

		print(doc._doc_)

*	查看内置文档字符串(doc两边是两个短下划线）

		import sys
		print(sys.__doc__)	#模块的可读说明
		print(sys.getrefcount.__doc__)	#模块内函数的说明
		print(int.__doc__)	#读取系统内置函数的说明

*	help函数

		help(str.encode)	#取得内置类型的help信息，使用类型名称dict,str,list
		help(bytes.decode)

