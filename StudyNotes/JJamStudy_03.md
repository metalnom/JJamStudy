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
# **03**
### Variables 1

---
# Variables 1
- 변수(variable)란?  **데이터를 담는 그릇**
- 기본 데이터 타입
    ``` python
    # 식별자 = <데이터>

    a = 10         # int
    b = 3.14        # float
    c = True        # bool
    d = "Python"    # str 

    print(type(a), type(b), type(c), type(d))  
    ```
---
# Variables 1
- 식별자
    - 변수, 함수, 클래스, 모듈 등의 이름
    - 식별자 규칙
        - 문자, 숫자, 밑줄 기호(_)를 이용
        - 숫자로 시작하면 안됨
        - 공백은 포함안됨
        - 밑줄 이외의 기호는 사용불가
        - 예약어 사용불가

---
# Variables 1
- 문자열 데이터 타입의 주요 함수
```python
f = "  python"
g = 'CLASS  '
h = f + ' ' + g

f.upper()
g.lower()
h.strip()
h.replace("PYTHON", "Funny")

dir(h)
```

---
# Variables 1
- 문자열의 오프셋 인덱스
    - 문자열은 순서가 있는 '문자'들의 집합
``` python
# 변수명[<시작idx>:<종료idx>:<간격>]
numbers = "123456789"
print(numbers[2])
print(numbers[-3])

print(numbers[2:5])
print(numbers[2:8:2])

print(numbers[::-1])
```