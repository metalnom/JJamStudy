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
# **06**
### Variables 2

---
# Variables 2
- List
    - 대괄호(**[]**) 사용
    - 다양한 자료형을 항목으로 가질 수 있음
    - 각 항목이 다른 자료형이라도 가능
``` python
lst = ['Song', 'Nam', 'Jung', 'Kim', 'Park']
lst_mix = [92, '파이썬', True, lst]
lst_num = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]

print(type(lst_mix))
```

---
# Variables 2
- List
``` python
lst_merge = lst + lst_mix   # 결합
print(lst_merge)

print(lst_num[2:8:2])       # 슬라이싱 [시작:끝:간격]

del lst_num[5]              # 항목 삭제
print(lst_num)

print(70 in lst_num)        # 항목 존재 여부
print(110 in lst_num)
```

---
# Variables 2
- List
    - method : List 데이터형에서 사용할 수 있는 함수
``` python
lst_num.append(110)                # 마지막에 항목 추가
lst_num.insert(6, '칠십오')         # 특정 위치에 항목 추가
lst_num.remove(80)                 # 입력값과 일치하는 항목 삭제
lst_num.pop()                      # 마지막 항목을 반환하고 삭제
lst_num.index(30)                  # 입력된 인자와 일치하는 항목의 위치 반환
lst_num.count(50)                  # 입력된 인자와 일치하는 항목의 개수 반환
lst_num.sort()                     # 리스트 항목을 오름차순으로 정렬
lst_num.reverse()                  # 리스트 항목을 내림차순으로 정렬
```

---
# Variables 2
- Tuple
    - 소괄호(**()**) 사용 혹은 사용하지 않고 항목 입력
    - 다양한 자료형을 항목으로 가질 수 있음
    - 각 항목이 다른 자료형이라도 가능
    - **단, 한 번 입력하면 항목을 변경할 수 없음!!**
``` python
tup1 = 10, 20, '삼십', False, lst
tup2 = (lst, '김', '이', '박')
print(tup1,  " >>> type : ", type(tup1))
print("{} >>> type : {}".format(tup2, type(tup2)))
```

---
# Variables 2
- Tuple
``` python
tup3 = (100, )              # 항목이 하나인 튜플을 생성할 때는 항목 뒤 ,
tup4 = 200, 

tup1[1] = 30                # 에러 발생. 생성된 튜플은 항목 변경 불가!!
del tup1[2]                 # 에러 발생. 생성된 튜플은 항목 삭제 불가!!

tup2.index('이')            # 입력된 인자와 일치하는 항목의 위치 반환
tup2.count('김')            # 입력된 인자와 일치하는 항목의 개수 반환
```

---
# Variables 2
- Set
    - 중괄호(**{}**) 사용
    - 다양한 자료형을 항목으로 가질 수 있음
    - 각 항목이 다른 자료형이라도 가능
    - **항목의 순서가 없고, 중복해서 쓸 수 없음**
``` python
set1 = {1, 2, '삼', 4, '오', 1}
print(set1)
print(type(set1))
```

---
# Variables 2
- Set
``` python
set2 = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
set3 = {3, 5, 7, 9, 11, 13, 15}

set2.intersection(set3)                     # 교집합
set2.union(set3)                            # 합집합
set2.difference(set3)                       # 차집합
```

---
# Variables 2
- List - Tuple - Set 간 타입 변환
``` python
a = [1, 2, 3, 4, 5, 5, 3, 2]

print(a, type(a), sep=' >> type : ')

b = tuple(a)
print(b, type(b), sep=' >> type : ')

c = set(b)
print(c, type(c), sep=' >> type : ')

d = list(c)
print(d, type(d), sep=' >> type : ')
```