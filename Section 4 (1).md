
![4.2.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.2.png)


```python
import random
num1 = random.randint(1,9)
num2 = random.randint(1,9)
num3 = random.randint(1,9)
print('what is ' + str(num1) + '+' + str(num2) + '+' + str(num3) + '= ?')
answer = num1 + num2 + num3
print(answer)
peopleanswer = input('please enter your answer:')
if str(answer) == peopleanswer:
    print('great!')
else:
    print('you are wrong')
```

    what is 6+1+5= ?
    12
    please enter your answer:12
    great!
    

![4.4.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.4.png)


```python
import random
num1 = random.randint(1,100)
num2 = random.randint(1,100)
print('what is ' + str(num1) + '+' + str(num2) + '= ?')
answer_ = num1 + num2
peopleanswer_ = input('enter your answer:')
if str(answer_) == peopleanswer_:
    print('正确')
else:
    print('错误')
```

    what is 85+3= ?
    enter your answer:88
    正确
    

![4.6.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.6.png)


```python
pounds = eval(input('Enter weight in pounds: '))
feet = eval(input('Enter feet:'))
inches = eval(input('Enter inches:'))

weight = pounds * 0.45359237
height = (inches * 2.54) + (feet * 12 * 2.54)
BMI = weight / (height ** 2 ) * 10000
print('BMI is ' + str(BMI) + '\nYou are Normal')

```

    Enter weight in pounds: 140
    Enter feet:5
    Enter inches:10
    BMI is 20.087702275404553
    You are Normal
    

![4.8.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.8.png)


```python
#定义接收三个整数
a = input('Please enter first numbers: ')
b = input('Please enter second numbers: ')
c = input('Please enter third numbers: ')
#定义最大值，中间值，最小值存放变量
min_ = 0
medium = 0
max_ = 0
#判断 最小的数
if a < b and a < c:
    min_ = a
elif b < a and b < c:
    min_ = b
elif c < a and c < b:
    min_ = c
#判断中间数
if b < a < c or c < a < b:
    medium = a
elif a < b < c or c < b < a:
    medium = b
elif a < c < b or  b < c < a:
    medium = c
#判断最大值
if a > b and a > c:
    max_ = a
elif b > a and b > c:
    max_ = b
elif c > a and c > b:
    max_ = c
#输出
print(str(min_) + ',' + str(medium) + ',' + str(max_))

```

    Please enter first numbers: 56
    Please enter second numbers: 42
    Please enter third numbers: 79
    42,56,79
    

![4.10.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.10.png)


```python
import random
a = random.randint(1,100)
b = random.randint(1,100)
print('what is ' + str(a) + ' * ' + str(b) + '?')
sum_ = a * b
answer = input('enter  your answer:')
if answer == str(sum_):
    print('True')
else:
    print('False')
```

    what is 100 X 55?
    

![4.12.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.12.png)


```python
number = eval(input('输出一个整数：'))
if number % 5 == 0 and number % 6 == 0:
    print('能被5和6整除')
elif number % 5 == 0 and number % 6 != 0:
    print('只能被5整除')
elif number % 6 == 0 and number % 5 != 0:
    print('只能被6整除')

```

    输出一个整数：6
    只能被6整除
    

![4.14.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.14.png)


```python
import random
coin = random.randint(1,3)
coin_name = ''
if coin == 1:
    coin_name = '正面'
elif coin == 2:
    coin_name = '反面'
print(coin_name)
gamer_answer = input('请输出你的猜测（正面或者反面）：')
if gamer_answer == coin_name :
    print('猜对了！')
else:
    print('猜错了！')
```

    正面
    请输出你的猜测（正面或者反面）：正面
    猜对了！
    

![4.16.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.16.png)


```python
import random
i = random.randint(65,90)
print(chr(i))
```

    C
    

![4.18.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.18.png)


```python
rate = eval(input('please enter rate:'))
mode = eval(input('please enter mode(1:$-￥,2:￥-$):'))
money = eval(input('please enter money: '))
if mode == 0:
    finalmoney = money * rate
elif mode == 1:
    finalmoney = money / rate
print('money is ' + str(round(finalmoney,2)))
```

    please enter rate:6.81
    please enter mode(1:$-￥,2:￥-$):1
    please enter money: 10000
    money is 1468.43
    

![4.20.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/4.20.png)


```python
temperature = eval(input('enter the temperature :'))
speed = eval(input('enter the wind speed:'))
if temperature > -58 and temperature < 41 and speed >= 2:
    t = 35.74 + (0.6215 * temperature) - (35.75 * (speed ** 0.16)) + (0.4275 * temperature * (speed ** 0.16))
    print('the wind chill index is ' + str(round(t,5)))
else:
    print('error')
    
```

    enter the temperature :5.3
    enter the wind speed:6
    the wind chill index is -5.56707
    
