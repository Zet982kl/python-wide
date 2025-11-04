#字符串str ,需要加上单引号或双引号
name="tao"
print(name)
#格式化输出：
#1占位符，占据位置，不会被输出
#  %
#name="tao"
#print("我的名字：%s" % name)
#%d  整数（常用）
age=18
name="tao"
print("我的名字：%s,年龄： %d"%(name,age))
#%数字d 数字是指减去位数的空格 属出位数不足，用零不全
b=1234
print("%5d"%b)
#%f 符点数
a=1.2345
print("%f"%a)#默认后6位数
c=2.9999
print("%.2f"%c)  #.数字f  表示保留几位数，遵循4舍5入
# f格式化
name="tao"
age=18
print(f"我的名字是{name},我今年{age}岁了")
#1运算符
print(2*6)
print(3/9)
#1.2 整除 取商的整数部分
a=5
b=2
print(a//b)
#1.3   %只取余数部分
print(a%b)
#1.4  *取幂  m**n指 m的n次方
print(a**b)#幂是最高u先级
#赋值运算符
num1=3
num2=5
#将一个变量的值 赋给另一个变量
num3=num2
#print(num3)
#将运算的值赋给变量
totle=num3+num2
#print(totle)
#2.2  +=
a=1
#print(a)
#a=a+1
a += 1  #等效于a = a + 1

#例
n1=99 #成本价
n2=66  #利润
n3=n1+n2#售价
n1 += n2
#print(n1)

# -=
b=1
b -= 1
#print(b)

# *=
c=2
c *= 2
#print(c)
#纯数字不能用

# 3  input（prompt） prompt是提示，会在控制台显示



# 4.  \t 制表符，通常表示空4个字符，也称缩进
#print("姓名\t年龄\t电话")

#4.2  \n 换行符
#print("hahaha\nxixixi")

#4.3  \r 回车 表示将当前位置移到本行开头
#print("aut\roooo")

#4.4  \\ 反斜杠符号
#print("ccc\\\jjj")
#print(r"ccc\\\jjj")#  r原生字符串，默认取消转义



# if的格式
#例，用户从控制台输入成绩，如果满分，输出‘你真棒’，如果60分，输出‘你还要继续努力’
#score = input("请输入成绩")
#if score== '100':
    #print("你真棒")
#if score == '60':
    #print("你还要继续努力")


#比较关系运算符
#== 比较两个值是否相等，相等的话就返回为true(真），不等的话就返回为false(假）
# != 比较两个值是否相等，相等的话就返回为true(真），不等的话就返回为false(假）
a=999
b=888
#print(a!=b)
#print(a>b)


# 逻辑运算符

# and 左右两边都符合才为真
a="hhh"
b="ccc"
#if a=='hhh'and b=='ccc':
    #print("a和b都在哭")


# or 左右两边只需要一边符合都为真
fruit='苹果'#表示室友带回的水果
#if fruit=='苹果' or fruit=='西瓜':
    #print("带回来了水果")


# not 表示相反的结果
#print(3>6)
#print(not 3>6)


# if--else
#if a==999 :
    #print("你真棒")
#else:     #else后面不添加任何东西
   # print("还要继续努力")
    # 三目运算
    #基本格式；为真结果 if 判断条件 else 为假结果
a==7
b==2
print("a比b大") if a>b else print("a比b小")


#  if--elif结构
#  if——else 2选1    if--elif 多选1
# if--elif 格式：

# if 条件1:
#     满足条件1所做的事情
# elif 条件2：
#      满足条件2所做的事情
#elif  条件3：
#      满做条件3所做的事情

#例如
#score=70
#if score>100:
      #print("太牛逼了")
#elif   0<score<20:
      #print("太辣了")
#elif  20<score<50:
      #print("一般般")
#else:
      #print("分数无效")


#  if 嵌套基本格式
#if 条件1：
#   事情1
#if 条件2：
#    事情2
# else:
#    不能满足的条件

# 内层if判断和外层if判断都可以是if--else结构

#定义一个布尔型变量，表示是否有车票
ticket = True
temp = 38.6
if ticket == True :
      print("可以进站")
      if 36.6 < temp < 37.6:
            print("体温正常，可以进站")
      else:
            print("体温不正常，被抓走")
else :
      print("不能进站")


#  while循环
#基本语法： 定义初始变量
#while条件： 循环体 ，改变变量
#i=1  #定义一个初始值，从一开始，记录循环数
#while i<=50 :
      #print("好好学习，天天向上")
      #i +=1#每执行一次i的值就加1



# 死循环
#基本格式：
#while Ture:
    #循环体
#while True :
      #print("我是帅哥")



#while循环的应用：计算1+2+3+...+100的和
i=1  # 定义一个初始值，从一开始，计录循环次数
s=0  #定义一个变量，保存计算结果，最开始计算结果为零
while i<=100 :
      s += i
      i += 1
      #print("计算结果是：",s)# 循环内，输出计算结果
print("计算结果是：",s)



#while循环嵌套
#含义：
#一个while循环里面还有一个while循环
#基本格式：
#while 条件1：
    #循环体1
    #while 条件2：
       #循环体2
       #改变变量2
    #改变变量1
#缩进决定层级，严格控制缩进，最好自动缩进
#i=1 #定义一个变量外循环次数
#while i<=3 :
#      print(f"这是第{i}次外循环")
#      h=1 #定义一个初始值，表示内循环次数
#      while h<=5 :
 #           print(f"这是第{h}次内循环")
#            h +=1
#      i += 1



i=1
y=1
while i<=100 :
      y *= i
      i += 1
print("计算结果是：",y)


#for循环
# 基本格式：
#for  临时变量 in 可迭代对象 :
#   循环体
# 注意冒号和缩进

#例如
#str = 'love'  # 定义一个字符串
#可迭代对象就是要去遍历取值的整体，只需要记住字符串就是可迭代对象
#for i in str :
 #     print(i)
#  range()
# 用来记录循环次数，相当一个计数器
#for i in range(1,6) :   #从1开始，到6结束，包前不包后
#      print(i)
#range()里面只写一个数，这个数就是循环次数，默认从零开始


#for循环应用 ：1+2+3+.......+100的值
s = 0
for i in range(1,101) :
      s += i
print("计算结果是",s)


#break和continue关键字，都是专门在循环中使用的关键字
#只能放在循环内
#i=0
#while i <= 5 :
  #    i += 1
   #   print(f"我吃了{i}个苹果")
    #  if i== 3 :
    #        print("吃饱了，不吃了")
     #       break



 #continue
#i=0
#while i<=10 :
      #i += 1
      #print(f"我吃了{i}个苹果")
     # if i == 5:
           # print("有虫子，不吃了")
           # continue



for i in range(1,11) :
    print(f"我吃了第{i}个苹果")
    if i== 3 :
        print("有虫子，不吃了")
        continue



#unicode : 所有字符都是2个字节
#好处 ：字符与数字之间转换速度更快
#坏处 ：占用空间大



#utf-8 ：精确，对不同字符用不同长度表示
#好处 ：节省空间
#坏处 ：字符与数字之间转换速度慢，计算字符需要多个字符来表示

#字符串编码转换
#a='love'
#print(a,type(a))  #str,字符串是以字符为单位进行处理
#a1= a.encode()  # 编码
#print(a1)
#print(type(a1))  # 以字节为单位进行处理
#a2 = a1.decode()  #解码
#print(a2,type(a2))


st = "我是帅哥"
st1 = st.encode("utf-8")
print(st1,type(st1))
st2 = st1.decode("utf-8")
print(st2,type(st2))

# 字符数按常见操作
#  + 字符串拼接
print('10'+'10')
n1 = "我是"
n2 = "帅哥"
print(n1 + n2)
print(n1 , n2,sep="")


#  * 重复输出
#print('我是帅哥 \n' *5)
#print('& \n' *5)


#成员运算符：检查字符串中，是否包含了某个子字符串（即某个字符或多个字符）
# in 如果包含的话，返回true,不包含的话，返回false
# not_in  和上面的话相反
name = "taotao"
print('t'in name)
print('t' not in name)
print('m' in name) #也可以对中文使用


#下标
#python中下标从0开始
#作用 ：通过下标可以快速找到对应数据
#格式 ：字符串名【下标值】
name = 'taotao'
print(name [0])
print(name [1]) #取值的时候，不要超出下标范围
#从右往左数，下标从 -1 开始 -1 -2 -3 .....
print(name [-1])


# 切片
# 含义：对操作的对象截取其中一部分
# 语法：【开始位置：结束位置：步长】 # 不写步长，默认为1，步长大小决定切取间隔
# 包前不包后原则
tr = 'iopuy'
print(tr[0:3])
print(tr[:3])
print(tr[3:])
print(tr[0:5:2])


#字符串常见操作
# 查找
#find : 检测某个子字符串是否包含在字符串中，如果在，就返回这个字符串开始位置的下标，否则就返回-1
name = 'taotao'
print(name.find('o'))
print(name.find('tao')) #检测到第一个tao，t的下标为0
print(name.find('t',2))
print(name.find('t', 5)) #超出范围返回-1
print(name.find('t', 2,4))


#index() 检测某个字字符是否包含在字符串中， 如果在，就返回在这个字符串开始的下标，否则就报错
#将上面find改为index

#count()  返回某个子字符串在整个字符串中出现的次数，没有就返回0
name = 'taotao'
print(name.count('o'))
print(name.count('taotao'))
print(name.count('m'))
print(name.count('o',1,6))
print(name.count('t',1))


#判断
#startswith() 是否以某个子字符串开头，是的话就返回true,不是的话，就返回false,
#         如果设置了开始和结束位置下标，则在指定范围内检查
#和上面的相同，改个字母


#endswith()  和上面一样，只是检查结尾

#isupper() 检查字符串中，是否所有字母都为大写，是的话就返回true


#修改元素
#replace（） 替换
#replace(旧内容，新内容，替换次数)
name = '好好学习，天天向上'
print(name.replace('天','使',2)) #替换次数如果省略，则默认全部替换


# split() 指定分隔符来切字符串
st = 'hello,python'
print(st.split(','))


# capitalize() 第一个字符大写，其他都小写
st = 'taotao'
print(st.capitalize())

# lower() 大写字母转为小写
st = 'TAO'
print(st.lower())

# upper() 小写字母转为大写
st = 'tao'
print(st.upper())



# 列表
# 基本格式：
# 列表名 = [元素1 , 元素2 , .......]  元素之间的数据类型可以各不相同
li = [1, 'o', 3, 4]
print(li,type(li))
print(li[1])
print(li[0:3]) #列表也可以进行切片操作
#列表也是可迭代对象，可以 for 循环，遍历取值
for i in li :
    print(i)



#列表的常见操作
# 添加元素
# append()  extend()   insert()
li = [1, 'o', 3, 4]
#li.append('about')     # append 整体添加
#print(li)
#li.extend('about')    # extend 分开添加
#print(li)
li.insert(2,'about')  #  insert 在指定位置插入元素,指定位置如果有元素，
#                                        插入的元素就后移
print(li)



#修改元素
# 直接通过下标就可以修改
#li = [1, 'o', 3, 4]
#li[1] = 'e'
#print(li)



#查找元素
# in : 判断指定元素是否存在列表中，如果存在就返回true,不存在，就返回false
# not_in :和上面相反
# 例如
#while True:
    #name_list = ['帅哥', '美人', '丑人']
    #name = input('请输入你的名称')
    #if name in name_list :
           # print(f"这个{name}昵称已被占用，请更改")
    #else :
            #print(f"昵称{name}已被你使用")
           # name_list.append(name)
            #print(name_list)
            #break


# index : 返回指定数据所在位置的下标， 如果数据不存在就会报错
# count : 统计指定数据在当前列表出现的次数
# 跟字符中的用法相同


#删除元素
# del
li = [1, 'o', 3, 4]
del li[2]
print(li)


# pop 删除指定下标的数据
li = [1, 'o', 3, 4]
#li.pop() #默认删除最后一个元素
#print(li)
li.pop(2)
print(li)


#remove 根据元素的值进行删除
li = [1, 'o', 3, 4]
li.remove(1)
print(li) # 报错，列表中不存在这个元素 # 默认删除最开始的那个元素


#排序
# sort ：将列表按特定顺序排列，默认从小到大
li = [23,44,87,93,32,86]
li.sort()
print(li)


# reverse : 倒序排序
li = [23,44,87,93,32,86]
li.sort(reverse=True)
print(li)


#列表推导式
# 格式一 ： [表达式 for 变量  in 列表]
# 注意： in后面不仅可以放列表， 还可以放range() ,可迭代对象
li = [1, 2, 3, 4, 5]
[print(i*5) for i in li]
li = []
#例1  将1到6放进列表里
#for i in range(1,6):
    #print(i)
    #li.append(i)
#print(li)
# 例2
[li.append(i) for i in range(1,6)]
print(li)

#格式二  [表达式 for  变量  in 列表 if 条件]
# 把奇数放进列表
li = []
# 例1
#for i in range(1,11) :
    #if i % 2 == 1:
       # li.append(i)
#print(li)
# 例2
[li.append(i) for i in range(1,11) if i % 2 == 1]
print(li)


# 列表嵌套
li = [1, 2, 3, [4, 5, 6]]  #[4， 5， 6]是里面的列表
print(li[2])
print(li[3]) #取出里面的列表
print(li[3] [0]) #取出内列表中的元素


#元组 tuple
# 基本格式： 元组名 = (元素1，元素2，元素3.....)
# 所有元素包含在小括号内，元素与元素之间用逗号隔开，不同元素也可以是不同数据类型
tua = (1,) #只有一个元素的时候，末尾必须加上逗号，否则返回唯一的值的类型
print(type(tua))


# 元组与列表的区别
# 1 元组只有一个元素末尾必须加逗号，列表不需要
# 2 元组只支持查询操作，不支持增删改操作
tua = (1,2,3)
print(tua[2]) #元组也有下标，从左往右，从0开始
print(tua.index(2))


#应用场景
#函数的参数和返回值
#格式化输出后面的（）本质上就是一个元组
name ='taotao'
age=18
print(f'{name}的年龄是{age}')



#字典
#字典格式： 字典名={键1：值1 ，键2：值2} #键和值之间用冒号隔开    #键值对之间用逗号隔开
dic = {'name' : 'taotao', 'age' : 18}
print(dic)
#字典中的键具备唯一性，但是只可以重复  #键名重复不会报错，后面的键会覆盖前面的


#字典常见操作
#查看元素
#变量名[键名]
dic = {'name' : 'taotao', 'age' : 18}
print(dic[‘name'])  #字典中没有下标，查找元素可以根据键名   #没有的键名报错
print(dic['age'])
#变量名 get(键名)
print(dic.get('age'))
print(dic.get('name'))#键名不存在，返回none


#修改
#修改元素
dic = {'name' : 'taotao', 'age' : 18}
dic['age'] = 20
print(dic)

#添加元素
#变量名【键名】= 值
#键名存在就修改，不存在就添加
dic = {'name' : 'taotao', 'age' : 18}
dic['high'] = 188
print(dic)


#删除元素
#del
#删除整个字典 ：del 字典名
#dic = {'name' : 'taotao', 'age' : 18}
#del dic
#print(dic)  #如果报错，已经被删除
#删除指定键值对，键名不存在就会报错，  del 字典名【键名】
#dic = {'name' : 'taotao', 'age' : 18}
#del dic['age']
#print(dic)
#clear() 清空字典里的东西，但保留了这个字典
#ic = {'name' : 'taotao', 'age' : 18}
#dic.clear()
#print(dic)
# pop() 删除指定键值对，键不存在就会报错
dic = {'name' : 'taotao', 'age' : 18}
dic.pop('age')
print(dic)


#len（）求长度
dic = {'name' : 'taotao', 'age' : 18}
print(len(dic))
li = (1,2,3,4)
print(len(li))
st = ('a','b','c')
print(len(st))

#keys()  返回字典里的所有键名
dic = {'name' : 'taotao', 'age' : 18}
print(dic.keys())
for i in dic.keys():
    print(i)



#values() 返回字典里面的所有值
dic = {'name' : 'taotao', 'age' : 18}
print(dic.values())
#2
for i in dic.values():
    print(i)


#items()  返回字典里的所有键值对，键值对以原组形式
dic = {'name' : 'taotao', 'age' : 18}
print(dic.items())
#
for i in dic.items():
    print(i)



#字典的应用场景
#使用键值对，存储描述一个物体的相关信息



#集合的基本格式：集合名 = {元素1，元素2，元素3......}
#集合具有无序性
#s1 = {'a','b','c','d','e'}
#print(s1)
#s2 = {1,2,3,4,5}
#print(s2)  #数字运行结果一样


#集合无需的实现方式涉及hash(哈希)表
#print(hash('a'))
#print(hash('b'))
#print(hash('c'))
#每次运行结果不同，hash值不同，那么在hash中的位置也不同，这就实现了集合的无序性
#print(hash(1))
#print(hash(2))
#print(hash(3))  #python中int整型的hash值就是它本身，在hash表中的位置不会发生变化，
                # 所以顺序也不会发生变化
#print(hash('999999'))# 数字加上引号变成字符串类型，会无序
# 无序性：不修改集合中的值


#集合具有唯一性，可以自己去重
#s1 = {1,2,3,4,2}
#print(s1)



#集合的常见操作
#添加元素
#add 添加的是一个整体
#s2 = {1,2,3,4,5}
#s2.add(8)
#print(s2) #集合的唯一性，决定了如果需要添加的元素已经存在，就不进行任何操作
          #一次只能添加一个元素


# update 把传入的元素拆分，一个个放入集合
#s2 = {1,2,3,4,5}
#s2.update((7,8,9)) #元素必须是可以被我们for循环取值的可迭代对象
#print(s2)



#删除元素
#remove：选择删除的元素，如果集合中有就删除，没有就会报错
#s2 = {1,2,3,4,5}
#s2.remove(3)
#print(s2)


# pop
#s2 = {1,2,3,4,5}
#s2.pop()
#默认删除根据hash表排序后的第一个元素
#print(s2)


#discard:  需要选择要删除的元素，有的话就删除，没有的话就会不进行任何操作
#s2 = {1,2,3,4,5}
#s2.discard(2)
#print(s2)


#交集和并集
#交集 &
#含义：共有的部分
#a = {1,2,3,4,5}
#b ={3,5,7,9}
#print(a & b) # 没有共有的部分，返回空集合set()



#并集 |
#a = {1,2,3,4,5}
#b = {3,5,7,9}
#print(a|b)



# 类型转换
#int(): 转换为一个整数，只能转换由纯数字组成的字符串
# float --> int
#a = 1.9
#print(type(a))
#b = int(a)
#print(type(b))
#print(b) #浮点型强转整数型，会去掉小数点后面的数值，只保留整数部分
# str --> int
#print(int('123')) #如果字符串中有数字和正负号以外的字符就会报错
#print(int('-2')) #正负号不能放在后面



#用户从控制台输入，判断年龄
#while True:
 #age = int(input("请输入你的年龄"))
 #if age>= 18:   #input默认输入的是字符串类型
    #print("你成年了")
 #else:
    #print("未成年")



#float() 转换为一个小数
#print(float(1))   #会自动添加一位小数
# #如果字符串中有正负号，数字，正负号以外的符号则不支持转换


# str(): 转换为字符串类型，任何类型都可以转换为字符串
#n = 100
#print(n)
#n1 = str(n)
#print(n1,type(n1))
#
#st = str(-1.80)
#print(st,type(st))   #float转换成str会去除末尾为零的小数部分
#
#st = str([1,2,3,4,5])
#print(st,type(st))


#eval  用来执行一个字符串的表达式，并返回表达式的值
#print(10+10)
#print('10'+'10')
#print('10+10')
#print(eval('10'+'10'))
#整形和字符串不可以相加

#eval()可以实现list,dict,tuple和str之间的转换
#str-->list
#st1 = '[[1,2],[3,4],[5,6]]'
#print(type(st1))
#li = eval(st1)
#print(li,type(li))


#str-->dict
#st2 ="{'name':'taotao','age':18}"
#dic = eval(st2)
#print(dic,type(dic))
#eval() 非常强大，但是不够安全，容易被恶意修改数据，不建议使用


#list():将可迭代对象转换为列表
# 支持转换为list类型: str, tuple ,dict, set
#str-->list
print(list("abcde"))


#tuple --> list
print(list((1,2,3,4,5)))

#dict -->list  #字典转换为列表，只会转字典名
#例一
dic = {'name' : 'taotao', 'age' : 18}
print(list(dic))
#例2
print(list({'name' : 'taotao', 'age' : 18}))


#set --> list
print(list({'a','b','c','d','e','f','g','h'}))
#集合转换为列表，会先去重，再转换




#深浅拷贝
#赋值
li = [1,2,3,4,5]
print(li)
li2 = li  #将li赋值给li2
print('li',li)
print('li2',li2)
#给li列表新增元素
li.append(6)
print('li',li)
print('li2',li2)
#赋值，等于完全共享资源，一个值的改变会完全被另一个值共享


#浅拷贝（数据半共享）
#会创建新的对象，拷贝的一层的数据，嵌套层会指向原来的内存地址
import copy  #导入copy模块
li = [1,2,3,[4,5]]  #定义一个嵌套列表
li2 = copy.copy(li)  #浅拷贝
print('li',li)
print('li2',li2)
#查看内存地址
print('li内存地址:',id(li))
print('li2内存地址',id(li2)) #内存地址不一样，说明不是同一个对象
#li2.append(6)
#print('li',li)
#print('li2',li2)
#往嵌套列表添加元素
li[3].append(7)
print('li',li)
print('li2',li2)  #外层内存地址不同，但内层地址相同
# 优点：拷贝速度快，占用空间小，拷贝效率高



#深拷贝（数据完全不共享）
import copy #导入copy模块
li = [1,2,3,[4,5]]
li2 = copy.deepcopy(li)
print('li',li)
print('li2',li2)
#li.append(6)
#print('li',li)
#print('li2',li2)
li[3].append(7)
print('li',li)
print('li2',li2)
print('li',id(li[3]))
print('li2',id(li2[3]))  #深拷贝数据变化只影响自己本身，跟原来的对象没有关联


#可变类型  list  dict  set
#含义： 变量对应的值可以修改，但是内存地址不会发生改变
li = [1,2,3,4,5]
print('li现内存地址',id(li))
li.append(6)
print('li现内存地址',id(li))
#字典
dic = {'name' : 'taotao', 'age' : 18}
print('dic现存地址',id(dic))
dic['name'] = 'tiantian'
print(dic)
print('dic现存地址',id(dic))
#集合
set = {1,2,3,4,5}
print("set",id(set))
set.add(6)
print(set)
print("set",id(set))


#不可变对象
#含义 ：变量对应的值不能被修改，如果修改会生成一个新的值，从而分配新的内存空间
n = 10 #整型
print("n的原地址",id(n))
n = 19
print('n的现地址',id(n)) #修改n的值，就会生成新的值，重新赋给变量n

#字符串类型
st = 'hello'
print('st',id(st))
st = 'sb'
print('st',id(st))

#元组
tua = (1,2,3,4,5)
print('tua',id(tua))
tua = ('a','b','c')
print('tua',id(tua)) #前面所说的深浅对拷贝，只针对可变对象






#函数
#含义:将独立的代码块组成一个整体，使其具有特殊功能的代码集，在需要的时候再去调用
#作用：提高代码的实用性，是整体代码看上去更加简练
#基本格式
#定义函数
#def 函数名():
#   函数体
#调用函数
#函数名()
def login():
    print('这是登录函数')
login()
login()  #调用几次，函数里面的代码就会运行几次，每次调用的时候，函数都会从头开始执行

#编写一个打招呼函数并调用它
def say_hello():
    print('hello')
    print('taotao')
    print('18')
say_hello()
say_hello()  #调用函数前，必须保证函数已经存在


#返回值
#函数执行结束后，最后给调用者一个结果
#作用：
#return会给函数的执行者返回值
def buy():
    return '一桶水果茶',20  #return返回多个值，以元组的形式返回给调用者
    return '20' #函数中遇到return下面的代码不会执行
print(buy())
#函数中遇到return，表示函数结束，不继续执行

#返回值的三种情况
# 一个返回值都没有，返回的结果是none
# 一个返回值，就把值返回给调用者
# 多个返回值，以元组的形式返回给调用者


#return与print的区别
# 1 return表示函数结束，print会一直执行
#def funa ():
    #return 123
#print(funa())
# 2 return是返回计算值，print是打印结果
#def add():
   # a = 1
    #b = 2
   # return a + b
#print(add())


#参数
#定义格式
#def 函数名(形参a，形参b):    #形参：定义函数时，小括号里面的变量
#     函数体
#   ...(如a=1,b=2)
#调用格式：
# 函数名(实参1，实参2)  #实参：调用函数时，小括号里面的具体值
#def add(a,b):
 #   return a + b
#print(add(1,3))   #1和3就是实参



#必备参数（位置参数)
#含义：传递和定义参数的顺序及个数必须一致
#  格式  def funa(a,b)：
def funa(name,name2,name3):
    print(name)
    print(name2)
    print(name3)
funa('tao','sst','bbt') #写了几个就必须传几个，不可以多传，也不可少传


#默认参数
#含义; 为函数提供默认值，调用函数时可不传该默认参数的值
#注意： 所有位置参数必须出现在默认参数前，包括函数定义和调用
#格式： def func(a=12):
def fsdh(a=5,b=2):
    print(b)
    print(a)
fsdh(10,4)
#设置了默认值，没有传值，会根据默认值来执行代码，传了值，根据传入值来执行代码



 #可变参数
 #含义：传入的值的数量是可以改变的，可以传入多个，也可以不传
 #格式：def func(*args)    args可以换成其他字符
def func(*args):
    print(args)
func(1,2)  #以元组形式输出



#关键参数
#格式： def func(**kwargs)
# 和可变参数一样，只不过以字典形式输出
def func(**kwargs):
    print(kwargs)
func(name='taotao',age=18)  #传值的时候，需要用键=值的形式
#作用：可以扩展函数的功能



#函数嵌套
#嵌套调用
# 含义：在一个函数里面调用另外一个函数
def study():
    print('晚上在学习')
def df():
    print('数学')
#调用
study()
print('数学')


#嵌套定义
#含义：在一个函数中定义另一个函数
def study():
    print('晚上在学习')
    def akl():
        print('数学')
    akl()
study()



#作用域
#含义：指的是变量生效的范围，分为两种，分别是全局变量和局部变量
#全局变量
#函数外部定义的变量，在整个文件中都是有效的
a = 100  #全局变量
def tes1():
    print('这是tes1中a的值:',a)
def tes2():
    global a
    a =120
    print('这是tes2中a的值:',a)
print('调用函数前a的值：',a)
tes1()
tes2()
print('调用函数后a的值',a)   #a的值没有被覆盖是因为函数内部如果要使用变量，会先从内部找，有的话就直接使用
                            #没有的话就从外面找



#局部变量
#函数内部定义的变量，从定义位置到函数定义结束位置有效
def funa():
    num =10  #局部变量
    print('num:',num)
funa()  #作用：在函数体内部，临时保存数据，即当函数调用完成后，就销毁局部变量

#在函数内部修改全局变量的值，可以使用global关键字
#global
#将变量声明为全局变量
#格式：global 变量名


#nonlocal
#作用：用来声明外层局部变量，只能在嵌套函数中使用
a =10
def outer():
    a =5
    def inner():
        nonlocal a
        a =20
        def inner2():
            nonlocal a
            a =30
            print('inner2中函数的值',a)
        inner2()
        print('inner函数中a的值',a)
    inner()
    print('outer函数中a的值',a)
outer()



#匿名函数
#基本语法
#函数名=lambda 形参：返回值（表达式）
#调用：结果=函数名（实参)
#普通函数
def add(a,b):
     return a+b
print(add(1,2))
#匿名函数
add = lambda a,b: a+b
print(add(1,2))


#lambda的参数形式
#无参数
funa = lambda:('炸弹')
print(funa())

#一个参数
funb = lambda name:'taotao'
print(funb('taotao'))

#默认参数
func = lambda name,age=18:(name,age)
print(func('taotao',20))

fune =lambda a,b,c=12:a+b+c
print(fune(1,2))

#关键字参数
fund = lambda **kwargs:kwargs
print(fund(name='taotao',age=18))


#lambda结合if判断
comp =lambda a,b:'a比b小'if a<b else'a比b大'
print(comp(1,2)) #lambda只能实现简单的逻辑，如果逻辑复杂且代码量较大，不建议用lambda
                       #会降低代码的可读性


#内置函数
#查看所有内置函数
#import builtins
#print(dir(builtins))
#大写字母开头是内置常量名，小写字母开头是内置函数名

#abs() 作用：返回绝对值
print(abs(-19))

#sum() 作用：求和
#函数里要放可迭代对象，字符串也不可以
print(sum([1,2,3,4,5]))


