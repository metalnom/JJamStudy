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
# **05**
### Conditional Syntax

---
# Conditional Syntax
- if 조건문 : **프로그래밍에서 매우 중요한 문법**
- 단일 조건에 따른 분기
``` python
if a > b:
    print('a가 b보다 큽니다.')
```
- 단일 조건 및 그 외 조건에 따른 분기
``` python
if a > b:
    print('a가 b보다 큽니다.')
else:
    print('a가 b보다 작습니다.')
```

---
# Conditional Syntax
- 여러 조건에 따른 분기
``` python
if a > b:
    print('a가 b보다 큽니다.')
elif a < b:
    print('a가 b보다 작습니다.')
else:
    print('a와 b가 같습니다.')
```

---

# [Mini Project] 메뉴판 만들기


![](./img/miniproj1-640x320.png) 

* input() 함수 활용
``` python
menu = input('메뉴를 선택하세요' : )
```
