# Python-24-
Python学习笔记(24)
# p77 字符串的常用操作_字符串的查询操作
s='hello,hello'
print(s.index('lo'))  #3
print(s.find('lo'))  #3
print(s.rindex('lo'))  #9
print(s.rfind('lo'))  #9
#index系列会抛异常，find系列会出-1，建议用-1



# p78 字符串的常用操作_字符串的大小写转换操作方法
s='hello,python'
a=s.upper()  #将整个字符串转大写
print(a,id(a))
print(s,id(s))  #字符串是不可变序列，只要转换为大写，将是一个新的字符串对象
print(s.lower(),id(s.lower()))
print(s,id(s))  #转换之后，会产生一个新的字符串对象，内容是向等的，id是不同的

s2='hello,Python'
print(s2.swapcase())  #使字符串大写变小写，小写变大写

print(s2,title())  #每个英文字母开头变成大写，其余变成小写



# p79 字符串的常用操作_字符串内容对齐操作的方法
s='hello,Python'
print(s.center(20,'*'))  #20是一行的总空间，*是填充物

print(s.ljust(20,'*'))  #所有填充符全在左侧
print(s.ljust(10))  #则不输出填充符
print(s.ljust(20))  #则全为空格

'右对齐'
print(s.rjust(20,'*'))
print(s.rjust(20))  #这里左侧有一块空白
print(s.rjust(10))  #这里就没有空白了

‘右对齐，使用0进行填充’
print(s.zfill(20))  #左边0填充
print(s.zfill(10))  #设计宽度小于原宽度返回原字符串
print('-8910',zfill(8))  #在减号右边和8910之间添加0
