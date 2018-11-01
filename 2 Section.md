
![2.1.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.1.png)


```python
import math
radius,length = eval(input('Enter the radius and length of a cylinder: '))
area = radius * radius * math.pi
volume = area * length
print('The area is '+ str(area) + '\nThe volume is ' + str(volume))
```

    Enter the radius and length of a cylinder: 5.5,12
    The area is 95.03317777109125
    The volume is 1140.398133253095
    

![2.2.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.2.png)


```python
pounds = eval(input('enter a value in pounds: '))
kg_ = pounds * 0.454
print(str(pounds) + 'pounds is ' + str(kg_) + ' Kilograms')
```

    enter a value in pounds: 55.5
    55.5pounds is 25.197 Kilograms
    

![2.3.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.3.png)


```python
number = eval(input('Enter a number between 0 and 1000 : '))
hundred = number // 100
ten = (number // 10) % 10
Singledigit = number % 10
sum_ = hundred + ten + Singledigit
print('The sum of the digits is '+ str(sum_))
```

    Enter a number between 0 and 1000 : 999
    The sum of the digits is 27
    

![2.4.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.4.png)


```python
water = eval(input('Enter the amuount of water in kilograms: '))
inital_temperature = eval(input('Enter the initial temperature: '))
final_temperature = eval(input('Enter the final temperature: '))
energy = water * (final_temperature - inital_temperature ) * 4184
print('The energy needed is '+ str(energy) )
```

    Enter the amuount of water in kilograms: 55.5
    Enter the initial temperature: 3.5
    Enter the final temperature: 10.5
    The energy needed is 1625484.0
    

![2.5.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.5.png)


```python
speed,acceleration = eval(input('Enter speed and acceleration: '))
length = (speed ** 2) / (2 * acceleration)
print('The minimum runway length for this airplane is '+ str(round(length,3))+ ' meters')
```

    Enter speed and acceleration: 60,3.5
    The minimum runway length for this airplane is 514.286 meters
    

![2.6.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.6.png)


```python
 print('a   b   a ** b\n1   2   '+str(1**2)+'\n2   3   '+str(2**3)+'\n3   4   '+str(3**4) +'\n4   5   '+str(4**5)+'\n5   6   '+str(5**6))
```

    a   b   a ** b
    1   2   1
    2   3   8
    3   4   81
    4   5   1024
    5   6   15625
    

![2.7.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.7.png)


```python
x1,y1,x2,y2,x3,y3 = eval(input('Enter three points for a triangle: '))
side1 = ((x2-x1)**2 + (y2-y1)**2)**0.5
side2 = ((x3-x2)**2 + (y3-y2)**2)**0.5
side3 = ((x1-x3)**2 + (y1-y3)**2)**0.5
s = (side1 + side2 + side3) / 2
area = (s * (s - side1) * (s - side2) * (s - side3)) ** 0.5
print('The area of the triangle is '+ str(round(area,1)))

```

    Enter three points for a triangle: 1.5,-3.4,4.6,5,9.5,-3.4
    The area of the triangle is 33.6
    

![2.8.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.8.png)


```python
v0,v1,t = eval(input('enter v0 , v1 and t :'))
a = (v1 - v0) / t
print('The average acceleration is '+ str(round(a,4)))
```

    enter v0 , v1 and t :5.5,50.9,4.5
    The average acceleration is 10.0889
    

![2.9.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.9.png)


```python
import time
currentTime = time.time()
totalSeconds = int(currentTime)
currentSeconds = totalSeconds % 60
totalMinutes = totalSeconds // 60
currentMinute = totalMinutes % 60
totalHours = totalMinutes // 60
currentHour = totalHours % 24

gmt_user = eval(input('Enter the time zone offset to GMT:'))
user_hour = currentHour - gmt_user
print('Current time is ',user_hour,':',currentMinute,':',currentSeconds,'GMT')
```

    Enter the time zone offset to GMT:-5
    Current time is  12 : 39 : 38 GMT
    

![2.10.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2.10.png)


```python
balance,rate = eval(input('Enter balance and interest rate(e.g., 3 for 3%):'))
interest = balance * (rate / 1200)
print('The interest is '+ str(round(interest,5)))
```

    Enter balance and interest rate(e.g., 3 for 3%):1000,3.5
    The interest is 2.91667
    

![2-12.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2-12.png)


```python
import turtle
#定义画笔
turtle.pencolor('black')
turtle.pensize(3)
turtle.speed(5)
side = 24 #总边数
now_side = 0 #现在的边数
sum_all = 10 #总个数
sum_now = 0 #现在的个数
rangle = -180 #下一个六边形的角度
point = -180 # 下一组六边形的坐标
#绘制
turtle.penup()
turtle.goto(0,0)
turtle.right(-30)
turtle.pendown()
while now_side < side:
    turtle.right(60)
    turtle.forward(100)
    now_side = now_side + 1
    if now_side % 6 ==0:
        turtle.right(rangle)
    if now_side % 12 ==0 :
        turtle.penup()
        turtle.goto(point,0)
        point = point - 180
        turtle.pendown()
turtle.done()
```

![2-13.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/2-13.png)


```python
import turtle
import math
#定义画笔
turtle.pencolor('black')
turtle.pensize(3)
turtle.speed(5)
#获取圆的数据
centerx,centery,radius = eval(input('Enter center and radius for circle:'))
area = radius * radius * math.pi
#绘制
turtle.penup()
turtle.goto(centerx,centery)
turtle.pendown()
turtle.circle(radius)
turtle.penup()
turtle.goto(centerx,radius)
turtle.pendown()
turtle.write(area)
turtle.done()
```
