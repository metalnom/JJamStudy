---
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.jpg')
marp: true
---

![bg left:60% 60%](https://www.python.org/static/community_logos/python-logo-inkscape.svg)


# **JJamStudy**
# **09**
### Function 1

---
# Function 1
- Parameter와 Return이 없는 함수
    - 반복되는 코드를 하나의 함수로 정의
    - 코드를 간결하고 보기 좋게
    - 함수의 이름으로 내용을 유추할 수 있게

``` python
def func_1():                         // 함수 정의
    print("=====< 메 뉴 >=====")
    print("    1. 한  식")
    print("    2. 중  식")
    print("    3. 양  식")

func()                              // 함수 사용
```

---
# Function 1
- Parameter는 있고 Return이 없는 함수
    - 인자를 받아서 함수 내에서 처리
    - 함수 내 처리 결과를 반환하지 않음
    - 인자를 받아 출력처리하는 등으로 활용

``` python
def func_2(dict):                   // 함수 정의
    print(dict[1])
    print(dict[2])
    print(dict[3])
    print(dict[4])

func_2(menu)                        // 함수 사용
```

---
# Function 1
- Parameter와 Return이 모두 있는 함수
    - 인자를 받아 처리한 결과를 return <변수명> 형식으로 반환
    - 전형적인 y=f(x) 구조

```python
def func_3(a, b):
    sum = a + b
    mul = a * b
    return sum, mul

c, d = func_3(a, b)
print('덧셈: {}, 곱셈: {}'.format(c, d))   
```

