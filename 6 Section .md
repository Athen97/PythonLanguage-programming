
![6.2.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.2.png)


```python
def sumDigits(n):
    hundred = n // 100
    ten = ( n // 10 ) % 10
    single = n % 10
    sum_ = hundred + ten + single
    print(sum_)
sumDigits(234)
```

    9
    

![6.4.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.4.png)


```python
def reverse(number):
    Thousand = number // 1000
    hundred = ( number // 100 ) % 10
    ten = ( number // 10 ) % 10
    single = number % 10 
    sum_ = ( single * 1000 ) + ( ten * 100 ) + ( hundred * 10 ) + Thousand
    print(sum_)
reverse(3456)
```

    6543
    

![6.6.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.6.png)


```python
def displayPattern(n):
    for row in range(1, n + 1):
        # Print spaces
        for i in range(row, n):
            print("  ", end = "")

        # Print numbers
        for i in range(row,0,-1):
            print(" " + str(i), end = "")

        print()
displayPattern(4)
```

           1
         2 1
       3 2 1
     4 3 2 1
    

![6.8.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.8.png)


```python
def celsiusToFahrenheit(celsius):
    print('Celsius    Fahrenheit\n')
    for celsius in range(40,30,-1):
        fahrenheit = celsius * 9 / 5  + 32
        celsius -= 1
        print('%d         %d   ' %(float(celsius),round(fahrenheit,2)))
def FahrenheitToCelsius(fahrenheit):
    print('Fahrenheit    Celsius\n')
    for Fahrenheit in range(121,30,-1):
        Celsius =  ( 5 / 9 ) * (Fahrenheit - 32)
        Fahrenheit -= 1
        print('%d         %d   ' %(float(Fahrenheit),round(Celsius,2)))
celsiusToFahrenheit(31)
FahrenheitToCelsius(30)
```

    Celsius    Fahrenheit
    
    39         104   
    38         102   
    37         100   
    36         98   
    35         96   
    34         95   
    33         93   
    32         91   
    31         89   
    30         87   
    Fahrenheit    Celsius
    
    120         49   
    119         48   
    118         48   
    117         47   
    116         47   
    115         46   
    114         46   
    113         45   
    112         45   
    111         44   
    110         43   
    109         43   
    108         42   
    107         42   
    106         41   
    105         41   
    104         40   
    103         40   
    102         39   
    101         38   
    100         38   
    99         37   
    98         37   
    97         36   
    96         36   
    95         35   
    94         35   
    93         34   
    92         33   
    91         33   
    90         32   
    89         32   
    88         31   
    87         31   
    86         30   
    85         30   
    84         29   
    83         28   
    82         28   
    81         27   
    80         27   
    79         26   
    78         26   
    77         25   
    76         25   
    75         24   
    74         23   
    73         23   
    72         22   
    71         22   
    70         21   
    69         21   
    68         20   
    67         20   
    66         19   
    65         18   
    64         18   
    63         17   
    62         17   
    61         16   
    60         16   
    59         15   
    58         15   
    57         14   
    56         13   
    55         13   
    54         12   
    53         12   
    52         11   
    51         11   
    50         10   
    49         10   
    48         9   
    47         8   
    46         8   
    45         7   
    44         7   
    43         6   
    42         6   
    41         5   
    40         5   
    39         4   
    38         3   
    37         3   
    36         2   
    35         2   
    34         1   
    33         1   
    32         0   
    31         0   
    30         0   
    

![6.12.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.12.png)


```python
def printChars(ch1,ch2,numberPerLine):
    i = 1
    for i in range(ch1,ch2+1):
        
        if i % numberPerLine == 0:
            print(i)
        else: 
            print(i,end='  ')
        i += 1
printChars(1,16,4)
        
```

    1  2  3  4
    5  6  7  8
    9  10  11  12
    13  14  15  16
    

![6.14.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.14.png)


```python
def m(i):
    pi = 0
    sign = 1
    for i in range(1, i + 1, 1):
        pi += sign / (2 * i - 1) 
        sign = -1 * sign
    print(round(4*pi,4))
mathpai(101)
```

    3.1515
    

![6.16.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.16.png)


```python
def numberOfDaysInYear(year):
    for year in range(2010,2021):
        if year % 4 == 0 and year % 100 != 0:
            print('%d 有366 天'%(year))
        else:
            print('%d 有365 天'%(year))
numberOfDaysInYear(2010)
```

    2010 有365 天
    2011 有365 天
    2012 有366 天
    2013 有365 天
    2014 有365 天
    2015 有365 天
    2016 有366 天
    2017 有365 天
    2018 有365 天
    2019 有365 天
    2020 有366 天
    

![6.18.png](https://github.com/poolbreak/PythonLanguage-programming/blob/master/images/6.18.png)


```python
import random
def printMatrix(n):
    for i in range(0,n**2):
        a = random.randint(0,1)
        i += 1
        if i % n == 0:
            print(a)
        else:
            print(a,end=' ')
printMatrix(3)
```

    0 1 1
    1 1 1
    1 1 0
    
