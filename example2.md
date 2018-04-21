## 시퀀스 자료형(1)
1.시퀀스 자료 인덱싱
```python
strdata = 'Time is money!!'
print(strdata[5])       #'i' 출력
print(strdata[-1])      #'!' 출력
print(strdata[-3])      #'y' 출력
print(strdata[-15])     #'T' 출력
```
```python
listdata = [1,2,[1,2,3]]
print(listdata[-1])         #[1,2,3] 출력
print(listdata[2][-1])      #3 출력
```
음수 인덱스가 가능하다. `strdata[-1]`이면 끝에서 첫 번째라는 의미이다.

2.시퀀스 자료 슬라이싱
```python
strdata = 'Time is money!!'
print(strdata[1:5])     #'ime' 출력
print(strdata[:7])      #'Time is' 출력
print(strdata[9:])      #'oney!!' 출력
print(strdata[-3:])     #'y!!' 출력
print(strdata[:])       #'Time is money!!' 출력
print(strdata[::2])     #'Tm smny!' 출력
```
[시작 인덱스:끝인덱스:스탭]<br>
시작인덱스 <= [시작인덱스:끝인덱스] < 끝인덱스