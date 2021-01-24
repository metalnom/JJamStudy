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
# **02**
### print함수

---
# print()
- 기본적인 출력 함수
``` python
print('Hello World')
```
- Separator 옵션
```python
print('A', 'B', 'C', sep=' ')
print('A', 'B', 'C', sep='-')
print('A', 'B', 'C', sep='\n')
print('A', 'B', 'C', sep='\t')
```
---
# print()
- End 옵션
``` python
print('Line1')
print('Line2')
print('Line3')

print('Line1', end=' ')
print('Line2', end=' ')
print('Line3')

print('Line1', end='\t')
print('Line2', end='\t')
print('Line3')
```

---
# print()
- format
``` python
print('%s is %s' % ('Python', 'Easy'))
print('{} is {}'.format('Python', 'Easy'))
print('{0} is {1}'.format('My Name', 'Changdo'))
print('{1} is {0}'.format('My Name', 'Changdo'))
print('{var1} is not {var2}'.format(var2='Difficult', var1='Python'))

print('Num1 = %5d, Num2 = %4.2f' % (9876, 1234.5678))
print("Num1 = {0:5d}, Num2 = {1:4.2f}".format(9876, 1234.5678))
print("Num1 = {a:10d}, Num2 = {b:10.3f}".format(a=9876, b=1234.5678))
```

---
# Comments
- 주석
    - 실행하고 싶지 않은 코드 앞에 #를 입력
    - 코드에 대한 설명을 넣고 싶을 때 주로 활용
    - 단축키 : ctrl + /
``` python
#print('Hello World')
print('Goodbye')
print('See you next time.')
# 오늘 수업은 여기까지 입니다.
# 수고들 하셨습니다.