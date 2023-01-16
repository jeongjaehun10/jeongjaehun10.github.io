# 정리


```python
math.sqrt(4)#.은 함수안에 출처밝혀야함 
x = np.linspace(0, 2*math.pi, 100) #0부터 2파이까지 100개의 숫자 
#sin 그래프의 x 값 
y = np.sin(x)
plt.plot(x, np.sin(x))
a.capitalize() # 맨첫글자만 대문자
a= "good morning"
a.title() #모든단어의 첫글자는 대문자 
#strip
a="    good morning   "
a.strip() #빈칸제거

a.rstrip()

a.split(',') # 콤마를 기준으로 자름

" - ".join(a)

" ".join('   LIFE-IS-SHORT,-WE-NEED-PYTHON   '.strip().split("-")).capitalize().replace('p',"P")

number = "three" # 넘버는 변수라는 걸 알려줘야함 
day = 3 # 넙버는 변수라고 지칭해줘야함 " " 문자열 
print("i ate {0} apples. so i had sicked for {1} days".format(number, day))

a={"apple":["사과", "능금", "백설공주"], "banana":"바나나","cherry":"체리"}

temp = input()

if int(temp) > 25:
    print("여름")
elif int(temp) > 15:
    print("가을")
elif int(temp) > 5:
    print("봄")
else:
    print("겨울") 
    
    for i in range(2, 10):
    print(f'{i}단입니다')
    for j in range(1, 10):
        print(f'{i} X {j} = {i * j}')
    print() 
```


```python
1+1
```




    2




```python
"""
print("hello")
print("good morning")

"""
```




    '\nprint("hello")\nprint("good morning")\n\n'




```python
for i in[1,2,3]:
    print(i)
    print("hello")
```

    1
    hello
    2
    hello
    3
    hello
    


```python
a=1
```


```python
a
```




    1



안녕하세요

글자출력은 마크다운 


```
파이썬은 들여쓰기가 중요하다 
```

# 제 1장 

## 제 1절

# 제2 장

## 칼럼만들기

## import 하기


```python
1+1
```




    2




```python
sqrt(4)# sqrt는 루트
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Input In [17], in <cell line: 1>()
    ----> 1 sqrt(4)
    

    NameError: name 'sqrt' is not defined



```python
import math
```


```python
math.sqrt(4)#.은 함수안에 출처밝혀야함 
```




    2.0




```python
import math as m # as는 자격 바꿈 
```


```python
m.sqrt(9)
```




    3.0




```python
from math import sqrt # 출처 안밝혀도 됨 
```


```python
sqrt(4)
```




    2.0




```python
import numpy as np
```


```python
np.sqrt(4)
```




    2.0




```python
math.sqrt(4)
```




    2.0




```python
pi
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Input In [12], in <cell line: 1>()
    ----> 1 pi
    

    NameError: name 'pi' is not defined



```python
math.pi
```




    3.141592653589793




```python
np.pi
```




    3.141592653589793




```python
from math import pi 
```


```python
pi
```




    3.141592653589793




```python
import matplotlib.pyplot as plt
```


```python
np.linspace(1, 10, 10) # 1부터 10까지 숫자를 10개 넣어라
```




    array([ 1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.,  9., 10.])




```python
# 9등분 같은 간격으로 
```


```python
np.linspace(1, 10, 3)# 3개간격으로 같은 길이 만큼 
```




    array([ 1. ,  5.5, 10. ])




```python
x = np.linspace(0, 2*math.pi, 100) #0부터 2파이까지 100개의 숫자 
#sin 그래프의 x 값 
y = np.sin(x)
plt.plot(x, np.sin(x))
```




    [<matplotlib.lines.Line2D at 0x203ad5f9a00>]




    
![png](output_35_1.png)
    



```python
x = np.linspace(0, math.2*pi, 100) #0부터 2파이까지 100개의 숫자 
#sin 그래프의 x 값 # 파이를 불러내야 하는데 math안에는 파이가 없음 
y = np.sin(x)
plt.plot(x, np.sin(x))
```


      Input In [22]
        x = np.linspace(0, math.2*pi, 100) #0부터 2파이까지 100개의 숫자
                               ^
    SyntaxError: invalid syntax
    



```python
plt.plot(x, y)
```


```python
x = np.linspace(0, 2*np.pi, 100) #0부터 2파이까지 100개의 숫자 
plt.plot(x, np.cos(x))
```


```python
x = np.linspace(0, 2*math.pi, 100)
plt.plot(x, np.cos(x))
plt.plot(x, np.sin(x))
```

# 데이터 타입

##  숫자
- 정수(integer) : int
- 소수(float) 둥둥 떠다니닌다. float 보통 업계에서는 실수


```python
a=3
a
```


```python
type(a)
```


```python
b=3.0
type(b)
```


```python
a=1+3.0
a # float 형으로 바꿈 
```


```python
int(3.1)
```


```python
float(3) # float 소수 실수 
```


```python
2**10
```


```python
11//4 # 몫
```


```python
11%4 #나머지 = 퍼센트 
```


```python
np.pi
```


```python
round(1.234) # 반올림 둥들게 # shift tap은 도움말 
```


```python
round(1.734, ndigits=2)
round(1.734, ndigits=3)# 출력은 마지막꺼만 출력
```


```python
import math
math.floor(1.234)# 내림
```


```python
math.ceil(1.234)# 올림 
```




    2




```python
print(math.floor(1.234)) # 두개 출력하는 법 
math.ceil(1.234)
```

    1
    




    2




```python
math.floor(1.56)
```




    1




```python
math.trunc(1.234)  # 버림 
```




    1



## 문자 
- string(str) 


```python
"hello" # 홑따옴표랑 쌍따옴표는 100%같음 
```




    'hello'




```python
a="hello"
a
```




    'hello'




```python
print(a) # 따옴표 없이 나옴 
```

    hello
    


```python
# seting 오토 클로즈 
```


```python
" '  ' " 
```




    " '  ' "




```python
print('그는 나에게 "사랑해요"라고 말했다.')
# 안에 쌍따옴표 있으니밖은 홑따옴표있으면 됨 
```

    그는 나에게 "사랑해요"라고 말했다.
    


```python
#"처분"이란 행정청이 구체적 사실에 관하여 행하는 법.
```

### 문자열의 연산


```python
a="Life is short." 
b="We need Python"
```


```python
a+b # 더하기가 아닌 이어 붙인 것이다.
```




    'Life is short.We need Python'




```python
a-b # 문자 문자는 빼기 안됨
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Input In [38], in <cell line: 1>()
    ----> 1 a-b
    

    TypeError: unsupported operand type(s) for -: 'str' and 'str'



```python
a*b # 곱하기 나누기 안됨 
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Input In [39], in <cell line: 1>()
    ----> 1 a*b
    

    TypeError: can't multiply sequence by non-int of type 'str'



```python
a*3 # 반복
```




    'Life is short.Life is short.Life is short.'




```python
"-"*40
```




    '----------------------------------------'




```python
print("-"*40)
print("커피가 나왔습니다.")
print("-"*40)
```

    ----------------------------------------
    커피가 나왔습니다.
    ----------------------------------------
    

### 문자열의 메소드 (method)


```python
a= "Hello"
```


```python
upper(a)# 파이썬에서 가로안에 넣은것은 편의이다.
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Input In [44], in <cell line: 1>()
    ----> 1 upper(a)
    

    NameError: name 'upper' is not defined



```python
a.upper() # a가 upper 대문자 
```




    'HELLO'




```python
print() # 파이썬은 객체 우선이다. 함수보다 
str()
```

    
    




    ''




```python
a.lower()
```




    'hello'




```python
a.capitalize() # 맨첫글자만 대문자
```




    'Hello'




```python
b=a.upper()
b.lower()

a.upper().lower().capitalize()
```




    'Hello'




```python
a= "good morning"
a.title() #모든단어의 첫글자는 대문자 
```




    'Good Morning'




```python
#a. # .tap은 함수 여러개 나옴 
```


```python
a.count('n')

# argument는 인수, 인자 
#parameter 매개변수 
```




    2




```python
len(a) #길이
```




    19




```python
#strip
a="    good morning   "
a.strip() #빈칸제거
```




    'good morning'




```python
print(a)
```

        good morning   
    


```python
a.rstrip()
```




    '    good morning'




```python
a.lstrip()
```




    'good morning   '




```python
#split()
a.split()
```




    ['good', 'morning']




```python
a=" good, morning, Hello"
a.split()
```




    ['good,', 'morning,', 'Hello']




```python
a.split(',') # 콤마를 기준으로 자름 
```




    [' good', ' morning', ' Hello']




```python
a=" good: morning: Hello"
a.split(':')
```




    [' good', ' morning', ' Hello']




```python
#join
a=["철수", "영희", "길동"]
"".join(a)
```




    '철수영희길동'




```python
"-".join(a)
```




    '철수-영희-길동'




```python
" - ".join(a)
```




    '철수 - 영희 - 길동'




```python
str(1) # 문자로 바꾸기 
```




    '1'




```python
int(1)
```




    1




```python
int("Hello")
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    Input In [72], in <cell line: 1>()
    ----> 1 int("Hello")
    

    ValueError: invalid literal for int() with base 10: 'Hello'


## 참거짓
- bool : boolean


```python
1<2
```




    True




```python
if 1 < 2 : 
    print("Yes")
```

    Yes
    


```python
if 1 < 2 : 
    print("Yes")
else: 
    print("No")
```

    Yes
    


```python
if 1 == 2 : 
    print("Yes")
else: 
    print("No")
```

    No
    


```python
1==2
```




    False




```python
if 1 : 
    print("Yes")
else: 
    print("No")  # 모든 숫자는 참거짓관점에서 모두 참 단한가지 0제외 
```

    Yes
    


```python
if 2 : 
    print("Yes")
else: 
    print("No")  
```

    Yes
    


```python
if 0 : 
    print("Yes")
else: 
    print("No")  #
```

    No
    


```python
bool(1<2)
```




    True




```python
bool(1)
```




    True




```python
if "Hello" : 
    print("Yes")
else: 
    print("No") # 모든 문자가 참이다. 
```

    Yes
    


```python
if "" : 
    print("Yes")
else: 
    print("No") #""은 문자중 유일하게 거짓이다.
```

    No
    


```python
a=np.array([1,2,3,4,5,]) #[]두개이상이면 대괄호 묶는것
```


```python
a=np.array(1,2,3,4,5)
a
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Input In [80], in <cell line: 1>()
    ----> 1 a=np.array(1,2,3,4,5)
          2 a
    

    TypeError: array() takes from 1 to 2 positional arguments but 5 were given



```python
a
```


```python
print(a)
```


```python
a>3
```


```python
a[a >3 ] # 무언가를 속아내고 싶을 떄 
```

- input()
- 일단 문자열을 출력해준다
- 출력은 항상 str 이다. 



```python
input()
```


```python
input("숫자를 입력해 주세요")
```


```python
#input의 아웃풋은 항상 문자열이다. 그래서 
#연산이 안됨 
```


```python
a = input("입력:  ")
b = input("두번째 입력:  ")
a+b
```


```python
a = input("입력:  ")
b = input("두번째 입력:  ")
a+b
```


```python
a = int(input("입력:  "))
b = int(input("두번째 입력:  "))
a+b
```


```python
a = input("입력:  ")
b = input("두번째 입력:  ")
a+b
int(a)+int(b)
```

숫자를 스트링으로만듬 str
- if, fof, class, def, for.... 마지막은 :
- factorial(5)
import math
math.factorial(input('정수 입력')


```python
import math
math.factorial(5)
```


```python
x=int(input("숫자를 입력: "))
if(x%2==1):
    print("홀")
else:    
    print("짝") 
```


```python
import math
math.factorial(int(input("정수 입력: ")))#5x4x3x2x1
```


```python
np.linspace(1,1000,4)
```


```python
import matplotlib.pyplot as plt
```


```python

x=np.linspace(0,2*math.pi)
y=np.sin(x)
z = np.cos(x)
plt.plot(x,y)
plt.plot(x,z)
```


```python
a='   LIFE-IS-SHORT,-WE-NEED-PYTHON   ' 
b=a.split() #리스트라서 join 안됨 
join
.replace('-',' ').lower().capitalize()

```


```python
a = '   LIFE-IS-SHORT,-WE-NEED-PYTHON   ' 
a.strip().replace('-',' ').lower().capitalize()
```


```python
" ".join('   LIFE-IS-SHORT,-WE-NEED-PYTHON   '.strip().split("-")).capitalize().replace('p',"P") 
```


```python
s= '   LIFE-IS-SHORT,-WE-NEED-PYTHON   ' 
ss= s.strip().capitalize().split('-')
ss
' '.join(ss) 
```


```python
from math import sqrt, factorial
```


```python
a = 1000 // 167
b = 1000 % 167

a+b 
```


```python
a=np.linspace(0,200,21) #0부터 10까지는 11가지
np.array(a)
```


```python
a = np.linspace(0,200,21)
b = a[a<=80]
b 
```


```python
a=["철수","영희","민수","아영" ]
"$".join(a)
```


```python
round(1.4567,ndigits=2)
```


```python
a= 'WezarezstudyingzPython'
a.split('z') 
```


```python
a = 'WezarezstudyingzPython'
a.replace('z', ' ') 
```


```python
a = [4,3,8,6,9]#리스트인데
for i in range(len(a)): #인덱스 4의 범위에서 출력함 
  if a[i] < 8 :
    print(a[i]) 
```


```python
a= np.array([4,3,8,6,9])
a[a<8]
```


```python
a = "  gOod$moRning   "
a.strip().replace('$', ' ').capiltalize()
```


```python
a = "  gOod$moRning   "
b= a.strip().lower().split('$')
c= ' '.join(b)
c.capitalize() 
```


```python
" ".join((a.strip().split("$"))).capitalize() 
```


```python
a = "  gOood$moRning   "
b =a.strip().lower().title().split('$')
' '.join(b) 
```


```python
a = int(input())
print(a*2) 
```


```python
words=input().split(",")
```


```python
words
```


```python
words = input().split()
words
```


```python
words=input().split(",")
words# 컴마로 분리해서 여러개 입력받기# 그냥 엔터침
```


```python
words=input().split(",")
words
```

## formatting 포맷팅


```python
print("i ate three apples. so i had sicked for 3days")
```


```python
number = "three" # 넘버는 변수라는 걸 알려줘야함 
day = 3 # 넙버는 변수라고 지칭해줘야함 
print("i ate number apples. so i had sicked for day days")
```


```python
number = "three" # 넘버는 변수라는 걸 알려줘야함 
day = 3 # 넙버는 변수라고 지칭해줘야함 " " 문자열
print("i ate {} apples. so i had sicked for {} days".format(number, day))
```


```python
number = "three" # 넘버는 변수라는 걸 알려줘야함 
day = 3 # 넙버는 변수라고 지칭해줘야함 " " 문자열 
print("i ate {0} apples. so i had sicked for {1} days".format(number, day))
```


```python
number = "three" # 넘버는 변수라는 걸 알려줘야함 
day = 3 # 넙버는 변수라고 지칭해줘야함 " " 문자열 
print("i ate {1} apples. so i had sicked for {0} days".format(number, day))
```


```python
# f- string f문자열
number = "three" # 넘버는 변수라는 걸 알려줘야함 
day = 3 # 넙버는 변수라고 지칭해줘야함 
print(f"i ate {number} apples. so i had sicked for {day} days")
```


```python
#이름과 나이를 입력받아서 name, age
name = "정재훈" 
age = 28
print(f"나의 이름은 {name}이고 나이는 {age}세 입니다.")
```


```python
name = input("이름")
age = input("나이")

print(f"나의 이름은 {name}이고 나이는 {age}입니다.") 
```

# 파이썬의 자료형
- 리스트, 튜플, 딕셔너리, 집합

# 리스트 <br>
- 만들기 크리에이트 c : [  ]
- 접근 리드 r
- 수정 업데이트u 
- 델리트d


```python
#만들기 #리스트는 여러개를 하나로 묶어줌 
a=[1,2,3,4 ]
a=[1,2,3,4, "Hello, Good Morning"]
a=[1,2,3,4, "Hello, Good Morning", [5,6,7,8,]] #nested list 중첩리스트
a
```


```python
type(a)
```


```python
a= 1,2# 안묶어도 이건 오류로 묶음 
a
```


```python
type(a)
```


```python
input()
```

- 접근 indexing / index(한개)한개를 콕콕 찍음


```python
a=[1,2,3,4, "Hello", "Good Morning", [5,6,7,8,]]
a
```


```python
a[1]
```


```python
a[0] # 시작숫자는 0부터다
```


```python
a[4]
```


```python
a[4][0]
```


```python
a[5][5] # 6번째글짜의 6번째
```


```python
a[6][2]
```


```python
#뒤에서 첫번째는 -1
a[-1]
```


```python
a[-2][-1]
```


```python
a[-0] # -0은 0이다. 
```


```python
a[4]+a[5]
```


```python
a[0:4] #a[start:stop] # stop의 수는 제외됨 
#접근 slicing start:stop
```




    array([1, 2, 3, 4])




```python
a[4:6]
```




    array([5])




```python
a[4:] # 끝까지 달림 
```




    array([5])




```python
a[:4]
```




    array([1, 2, 3, 4])




```python
a[:]
```




    array([1, 2, 3, 4, 5])




```python
a[-3: ]
```




    array([3, 4, 5])




```python
a[4][2:4] # 2부터시작하니까 뒤에 두글자 출력은 4-2는 2글자
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    Input In [87], in <cell line: 1>()
    ----> 1 a[4][2:4]
    

    IndexError: invalid index to scalar variable.



```python
#2<= <=100
#1<n<3 
#1<=n<3 2개 우리는 한쪽만 등호니까 갯수는 걍 빼면됨 
#1<= n <=3 3개
```


```python
a[5][5:] # 띄어쓰기도 세줌
```

- 수정


```python
#old one = new
a[1]= 22
a
```

- 추가


```python
a.append(9)
```


```python
a
```


```python
b =[]
for i in [1,2,3]
    b.append(i)
```


```python
a
```


```python
a.insert(2, 33)
a
```

- 삭제 


```python
a.remove(3)
a
```


```python
a.remove(9)
a
```


```python
a.pop(4) # hello 지운다
```


```python
a
```

- 정렬 sort(메소드 객체.sort이렇게) , sorted(파이썬 내장함수)


```python
a=[1,3,4,2]
```


```python
sorted([1,3,4,2])
```


```python
a=[1,3,4,2]
a.sorted()
```


```python
a=[1,3,4,2]
a.sort()
```


```python
a
```


```python
a.reverse()
```


```python
a
```

### tuple(튜플, 투플) list랑 99%같음
- list는 수정되는데 튜플은 수정이 안됨 
- 주민등록번호 같은 수정되면 안되는 것


```python
#만들기는 소괄호 () x튜를로 묶는것은 패킹
#푸는 것은 언패킹
a=(1,2,3,4)
```


```python
type(a)
```


```python
a= 5,6,7,8 # 소괄호 안해도 됨 
a
```


```python
a[0]
```


```python
a[0]=55
```


```python
num=(10,12)
```


```python
a, b#(언패킹)=num#(튜플)
print(a)
print(b)
```

### 딕셔너리(dictionary)
- 만들기: { : } 사전찾기 대응 
- 만들기 {KEY : VALUE}


```python
a={"apple":"사과", "banana":"바나나","cherry":"체리"}
```


```python
type(a) 
```

- 접근, 검색


```python
a['apple']
```


```python
a[0] # 인덱스인 숫자는 없음 
```


```python
a['사과'] #반대는 안됨
```


```python
a.keys() 
```


```python
a.values()
```


```python
a.items() # 대괄호 안에 튜플
```


```python
for i in a.items():
    print(i)
```


```python
for i, j in a.items(): # 사실은 (i, j)임 
    print(i, j)
```


```python
a={"apple":"사과", "능금", "백설공주", "banana":"바나나","cherry":"체리"}
```


```python
a={"apple":["사과", "능금", "백설공주"], "banana":"바나나","cherry":"체리"}
```


```python
a
```

- 수정


```python
a['banana'] ='빠나나'
```


```python
a
```

- 추가


```python
a["durian"]="두리안"
```


```python
a
```


```python
명단={"철수":"합격", "영희":"합격"}
name=input("이름을 입력하세요: ")
print(명단[name])
```


```python
명단={"철수":"합격", "영희":"합격"}
name=input("이름을 입력하세요: ")
print(f"{명단[name]}입니다")
```


int()
float()
str()
bool()

list()   []
tuple()  ()
dict()   {:}
set()    {}




```python
# 변수는 수가 아님 변수는 장독대 안에 여러개가 들어감
```


```python
a=1 # 등호가 아니라 시차가 있음 오른쪽먼저만들고 왼쪽들어감
b=2
c=a+b
a=a+1
```


```python
a= [1,2,3]
b=a
```


```python
b=a
b[2]=50
id(a)
```


```python

```


```python
id(a) # 노트에 가서 방번호 물음 
```


```python
b = a # 바로가기느낌이라 b수정되면 a도 수정
```


```python
b
```


```python
c=a.copy() # 완전히 새로 복사라 수정되도 괜춘
```


```python
c
```


```python
c[2]=30
```


```python
c
```


```python
a
```


```python
b[2]=300
```


```python
b
```


```python
a #
```


```python
id(a)
```


```python
id(b)
```


```python
id(c)
```


```python
a, b= ('python', 'life')
(a,b)='python', 'life'

a=b='python'
```


```python
a # 2장연습문제 
```

# 조건문 if

if 문의 구조
```
if 참거짓:
    참일 때 실행 될 문장 
elif:
    참일 때 실행 될 문장 
elif:
    참일 때 실행 될 문장 
else:
    나머지 모두 실행
```


```python
if 1<2:
    print("Yes")
```


```python
if 3<2:
    print("Yes")
else:
    print("No")
```


```python
if 1<2:
    print("Yes")
elif:             #else if 줄여서 
elif:
else:    
```

### temp=input()
#25보다 크면 "여름"
#15....크면 "가을"
#5도보다 크면 "봄"
#그이하 "겨울"

temp = int(input())
if temp > 25:
    print("여름")
elif temp > 15:
    print("가을")    
elif temp > 5:
    print("봄")     
else :
    print("겨울")


```python
temp = int(input())
# elif는 제외해준다. 
if temp > 25 : 
  print('여름')
elif temp > 15 :
  print('가을')
elif temp > 5 :
  print('봄')
else : 
  print('겨울') 
```


```python
temp = input()

if int(temp) > 25:
    print("여름")
elif int(temp) > 15:
    print("가을")
elif int(temp) > 5:
    print("봄")
else:
    print("겨울") 
```


```python
temp = int(input())

if temp > 25 : 
  print('여름')
if temp > 15 :
  print('가을')
if temp > 5 :
  print('봄')
else : 
  print('겨울') # 둘다 맞으니 둘다 실행 else는 아님
```


```python
number= int(input())

if number%2 ==0:
    print("짝수입니다.")
else:
    print("홀수 입니다") 

```


```python
if int(input('number = ')) % 2 == 0:
    print('짝수입니다')
else:
    print('홀수입니다') 
```


```python
#A in B #A가 B안에
if 'bill' in['coin', 'bill', 'card']:
    print("택시를 타자")
else:
    print("걸어가자")
```


```python
시장 = ['사과', '바나나', '배']

if '바나나' in 시장:
    print("구매한다")
else:
    print("구매 안한다")
```


```python
names=['영희', '전우치', '홍길동', '장길산']
name=input("이름을 입력해주세요")

if name in names:
    print('합격입니다')
else:
    print('불합격입니다')
```

# 반복문 for
- for 문의 구조
- for i in....:
- 반복할 문장 
- for i in[1,2,3]: 


```python
#for i in[1,2,3]: #in뒤에는 리스트
    print(i) # i가 1인상태에서 1개씩 다 시행 밑으로 
    # 다하면 올라가서 2 다 밑까지 마지막 까지 다가면 ..벗어나서
    # 마지막 포문을 실행시킴
    ...
    ...
    ...
    ...
```


```python
for i in [1,2,3]:
    print(i)
    print("Hello")
    print()

```


```python
for i in [1,2,3]:
    print()
    print("Hello")
    print()

```


```python
for _ in [1,2,3]:
    print()
    print("Hello")
    print()
```


```python
for i in [1,2,3,4,5,6,7,8,9,10]:
    print(i)
```


```python
for _ in range(10):
    print(_)
```


```python
for i in range(2,10):
    print(i)
```


```python
for i in range(1,11,3):
    print(i)
```


```python
for i in range(0,11,3):
    print(i)
```


```python
for i in range(0,11,2): # 0에서 2칸뛰면 2
    print(i)
```


```python
for i in range(10):
    print(i, end = ",  ")
```


```python
# 2부터 10까지 짝수만 출력
for i in range(2, 11, 2):
    print(i)
```


```python
for i in range(1, 11):
    if i%2 ==0:
        print(i)
```


```python
names
```


```python
for name in names:
    print(name)
```


```python
for i in range(4): # in안에있는 것중에 i를 출력
    print(names[i]) # names0 names1 names2 names3 

```

- 총합구하기


```python
for i in range(10):
    
sum =
1 = 0+1
3 = 1+2
6 = 3+3
10 =6+4
sum = sum +i #시차가 있음 
```


```python
sum = 0
for i in range(10):
    sum = sum+i #i만큼씩 
    print(sum)

```


```python
sum = 0
for i in range(10):
    sum = sum+i
print(sum) # 결과만 나옴 #0부터 9까지 더한값
```


```python
sum = 0
for i in range(1, 11):
    sum +=i  #i만큼씩, 문법적인 설탕 
print(sum)
```


```python
#234부터 567까지의 합은
sum =0
for i in range(234, 567+1):
    sum +=i  #i만큼씩, 문법적인 설탕 
print(sum)
```


```python
#234부터 567까지의 합은
#두수를 입력받아서 합은?
sum=0
for i in range(int(input()), int(input())+1):
    sum += i
print(sum)
```


```python
a=[]
for i in range(21):
    if i%2==1:
        a.append(i)
print(a)
```


```python
a=[]# i가 홀수인 경우에만 a에다가 추가
for i in range(21):
    if i % 2 == 1: a.append(i)
a 
```


```python
# 구구단 
for i in range(1, 10) : 
    print(f"2x{i} ={2*i}")#f랄 중괄호는 변수처리 1에서 10까지 범위
    #x는 단지 표시 실제는 *곱하는것 
```


```python
for i in range(2,10): # 2내려오고 j에서 1부터 9까지 다실행 시키고 
    for j in range(1, 10) : #다시 3내려와서 1부터 9까지 다실행
        print(f"{i}x{j} ={i*j}")
        
```


```python
for i in range(2, 10):
    print(f'{i}단입니다')
    for j in range(1, 10):
        print(f'{i} X {j} = {i * j}')
    print() 
```


```python
#파이썬 고유의 자료형 4가지
튜플 dictionary list set(집합)
```


```python
a = [1, 2, 3, 4, "Hello", "Good Morning"] 
a.remove(4) 
print(a)
```


```python
a=int(input())
n = 0
for i in range(1, a+1):
    n += i
print(i)

```


```python
a = int(input())
n = 0
for i in range(1, a+1):
    n += i
print(n) 
```


```python
result=[]
for i in range(1, 1001):
    if i%2==0:
        result.append.i
        print(result)
```


```python
result = []
for i in range(1000+1) :
  if i%2 == 0:
    result.append(i)

print(result) 
```


```python
a=[]
list(range(0, 1001,2)).
 
```


```python
a=[]
for i range(0, 10+1):
    a.append(i)
print(a)


```


```python
b=[i for i in range(0, 10+1)] #그대로 쓰고 앞에 원하는걸 얘기하고 뒤에
#수식하는 느낌 
b
```


```python
c=[i for i in range(0, 10+1) if i%2==0] #[]하는 이유는 리스트 모을꺼
c
```


```python
# 복사를 하는 3가지방법
a = [1,2,3]
b=a
c=a.copy()# 객체 뒤에 붙어있는게 메소드
d=a[:]

import copy
e=copy.copy(a)# 일반적 카피라는 함수를 씀 
```


```python
form copy import copy
e= copy(a)
```


```python


```


```python
a=[1,2,3,4,"Hello","Good Moring"]
a[5][5]
```


```python
a=[1,2,3,4,"Hello","Good Moring"]
a[5][5:]
```


```python
a=[1,3,4,2]
a.reverse()
print(a)#그냥 이렇게 하면 뒤집기만
```


```python
a=[1,3,4,2]
a.sort()
print(a)
```


```python
a=[1,3,4,2]
a.sort()
a.reverse()
print(a)
```


```python
a=sorted(a)
a.reverse()
```


```python
data = [[33, 37, 39, 31],["여자","여자","남자","여자"]]
average = 0
for i in range(0, 3 + 1):
    if data[1][i] == "여자":
        average += data[0][i]
print(average / 3) 
```


```python
data = [["영자", "옥순", "광수", "순자"],[33, 37, 39, 31],["여자","여자","남자","여자"]] 
sum = 0
count = 0
for i in range(len(data[2])):
    if data[2][i] == '여자':
    sum = sum + data[1][i]
    count = count + 1
mean = sum / count
print(mean) 
```


```python
numpy 
pandas 
matplotlib
```


```python
number = 0
for i in range(1, 5):
    number = number + i
print(number)    
```


```python
bool([])
```


```python
lambda(a: a*3, a)
```


```python

```
