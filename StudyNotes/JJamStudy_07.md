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
# **07**
### Loop Syntax 1

---
# Loop Syntax 1
- While 문
    - **프로그램을 지속적으로 On 시켜놓기 위해 필수적인 문법**
    - 특정 조건이 만족되는 동안 코드 블록을 반복 실행
``` python
# while <조건문>:
#     <코드블록>
i = 0

while i < 10:
    i = i + 1
    print('{}번째 입니다.'.format(i))   
```

---
# Loop Syntax 1
- 무한반복문, continue, break
``` python
i = 0

while True:            # True 혹은 1을 조건으로 하면 무한반복
    i += 1
    if i % 3 == 0:
        continue       # continue를 만나면 아래 코드는 실행 하지 않고 다시 반복    
    print(i)
    if i % 10 == 0:
        break          # break를 만나면 반복문을 종료함

print('반복문 종료!')
```

---
# Loop Syntax 1
- 연습문제
``` python
# 1 ~ 100 까지의 숫자를 더한 값을 구하시오.
i = 0
sum = 0

while i < 100
...

# 1 ~ 200 까지의 짝수를 더한 값을 구하시오.
```

---
# [MiniProject] 메뉴판 업그레이드 1
- While문 활용 무한반복
- 메뉴 선택 화면에서 0을 입력하면 프로그램 종료
- 메뉴를 여러 가지 선택할 수 있도록
- 메뉴는 리스트에 하나씩 추가하여 저장
- 마지막 화면에서는 리스트에 저장된 메뉴가 전부 출력
- 단, for문을 배우지 않았으므로 리스트 형태 그대로 출력함