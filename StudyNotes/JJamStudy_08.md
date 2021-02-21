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
# **08**
### Variables 3

---
# Variables 3
- Dictionary
    - 데이터 전체를 중괄호(**{}**)로 묶어 사용 
    - 하나의 데이터는 Key와 Value로 구성되어 있음
    - Key는 숫자나 문자열
    - Value는 다양한 자료형을 사용할 수 있음
``` python
dict = { key1:value1, key2:value2, key3:value3 }

menu = { 1:'한식', 2:'중식', 3:'양식'}
menu_c = { '짬뽕':8000, '짜장면':6000, '탕수육':12000 }
```
---
# Variables 3
- Dictionary
    - Key를 이용해 Value에 접근
    ``` python
    print(menu[2])
    print(menu['짬뽕'])         // 잘못된 Key인 경우 에러발생!
    print(menu.get('짬뽕'))     // 잘못된 Key인 경우에도 에러 발생하지 않음!
    ```
    - Value에 다양한 데이터 형식을 사용해 활용

    ``` python
    menu_k = {'한식':['김치찌개', '된장찌개', '비빔밥']}
    menu_kp = {'한식':{'김치찌개':6000, '된장찌개': 6000, '비빔밥': 5000}}
    ```

---
# Variables 3
- Dictionary
``` python
del menu[2]                 // Key에 해당하는 자료 삭제

print(menu.keys())          // 딕셔너리의 전체 Key를 리스트 형태로 반환
print(menu.values())        // 딕셔너리의 전체 Value를 리스트 형태로 반환
print(menu.items())         // 딕셔너리의 전체 Key와 Value 쌍을 튜플 형태로 반환

menu_add = {4:'분식'}
menu.update(menu_add)       // 딕셔너리에 딕셔너리 형식의 자료 추가
print(menu)

menu.clear()                // 딕셔너리의 모든 자료 삭제
```
