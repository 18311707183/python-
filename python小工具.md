```python
#1.冒泡排序
lis=[55,9,998,922,33,44,55,77,99]
def maopao():
    for i in range(len(lis)-1):
        for j in range(len(lis)-1-i):
            if lis[j]>lis[j+1]:
                lis[j],lis[j+1]=lis[j+1],lis[j]
    return lis
print(maopao())


# 2.计算x的n次方的方法
def power(x,n):
    s=1
    while n>0:
        n=n-1
        s=s*n
    return  s
print(power(0,5))

# 3.计算a*a + b*b + c*c + ……
def calc(*numbers):
    sum=0
    for n in numbers:
        sum=sum+n*n
    return sum
print(calc(4))


# 4、计算阶乘 n!
#方法1
def fac():
    num=int(input("请输入一个数字"))
    factorial=1
#先判断输入的数字是正数还是负数或者 0
    if num<0:
        print("负数没有阶层")
    elif num==0:
        print("0的阶层为1")
    else:
        for i in range(1,num+1):# 遍历出从1到输入数字的后面一个数
            factorial=factorial*i
            print("%d 的阶层为 %d"%(num,factorial))
#方法2
def factoeial(n):
    result=n
    for i in range(1,n):
        result *=i
    return result
#方法3
def fact(n):
    if n==1:
        return 1
    return n*fact(n-1)
print(fac())
print(factoeial(5))
print(fact(5))

```

