## 시퀀스 자료형(2)

1.시퀀스 자료 연결
```python
strdata1 = 'I love '; strdata2 = 'you'
print(strdata1 + strdata2)              #'l love you' 출력
listdata1 = [1,2,3]; listdata2 = [4,[5,6]]
print(listdata1 + listdata2)            #[1,2,3,4,[5,6]] 출력
```
자료형이 동일한 두개의 시퀀스 자료는 '+' 연산자로 순서있게 연결하여 새로운 시퀀스 자료를 만들 수 있다. 문자열 + 리스트와 같이 자료형이 다르면 '+'로 연결할 수 없다.<br>
(참고로 파이썬은 구문뒤에 세미콜론을 사용하지 않지만 한줄에 여러 구문을 쓰고 싶을 때는 세미콜론을 이용한다.)

2.시퀀스 자료 반복
```python
artist = '빅뱅'
sing = '뱅~'
dispdata = artist + '이 부르는 ' + sing*3
print(dispdata)             #'빅뱅이 부르는 뱅~뱅~뱅~' 출력
listdata = [1,2,3]
print(listdata*2)           #[1,2,3,1,2,3] 출력
```
seqdata*n 이면 seqdata가 n번 출력된다

3.시퀀스 자료 크기
```python
strdata = 'I love you'
print(len(strdata))         #10 출력
listdata  = ['a','b','c', strdata]
print(len(listdata))        #4 출력
print(len(listdata[3]))     #10 출력
```
4.멤버체크
```python
listdata = [1,2,3,4]
ret1 = 5 in listdata
ret2 = 4 in listdata
print(ret1)             #False
print(ret2)             #True
strdata = 'abcde'
ret3 = 'c' in strdata   
ret4 = 'l' in strdata   
print(ret3)             #True
print(ret4)             #False
```
in키워드로 자료에 어떤 값이 있는지 없는지 확인할 수 있다.<br>**<값> in <자료>**
