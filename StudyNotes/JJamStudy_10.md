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
# **10**
### Loop Syntax 2

---
# Loop Syntax 2
- For 문
    - **프로그래밍에서 가장 중요한 문법 중 하나**
    - 지정한 범위 동안 코드 블록을 반복
    - 반복 범위는 리스트 혹은 range()를 사용
``` python
for i in [0, 1, 2, 3, 6, 7]:
    print(i)

for i in range(0, 20, 2):           // range(start, end, step)
    print(i)
```

---
# Loop Syntax 2
- For 문
    - 반복가능한(iterable) 자료형을 범위로 지정 가능
``` python
student = ['Nam', 'Song', 'Jung', 'Kim']

for name in student:
    print(name)

for k in menu.keys():            // 딕셔너리의 key들만 차례대로 꺼냄 
    print(k)

for k, v in menu.items():        // 딕셔너리의 key와 value를 차례대로 꺼냄   
    print('{}:{}'.format(k, v))
```


---
# Loop Syntax 2
- 연습문제
    - 중복 for문을 사용하여 2단 ~ 9단 표현
``` console
2 x 1 = 2       3 x 1 = 3       4 x 1 = 4 ...
2 x 2 = 4       3 x 2 = 6       4 x 2 = 8 ...
2 x 3 = 6       3 x 3 = 9       4 x 3 = 12 ...
```

---
# [MiniProject] 메뉴판 업그레이드 2
- 함수를 활용하여 중복 구문을 정리
- 딕셔너리를 활용하여 각 메뉴의 이름과 가격을 저장
- for문을 활용하여 메뉴 출력 시 저장한 메뉴를  하나씩 출력
- 마지막에는 총 합계 금액을 출력
- (옵션1) 손님으로부터 금액을 받아 거스름돈을 계산하여 출력
- (옵션2) 계산 후 대기번호를 출력