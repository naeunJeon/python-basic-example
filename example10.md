## 파이썬 모듈 이해하기

코드를 작성할때 이미 만들어져 있는 함수들을 활용하면 보다 효율적이고 빠르게 개발할 수 있다. 이미 만들어져 있고 안정성이 검증된 함수들을 성격에 맞게 하나의 파이썬 파일에 묶어 만들어 놓은 것을 **모듈**이라고 한다.

외무 모듈에 있는 함수들을 활용하려면 이 모듈을 우리 코드로 가져와서 자유롭게 사용할 수 있도록 해야하는데 이런 일을 파이썬에서는 **모듈을 임포트 한다**고 한다.

```python
import time             #파이썬 내장 모듈인 time 모듈을 import 키워드를 통해 임포트

print('5초간 프로그램을 정지합니다.')
time.sleep(5)           #함수이름 앞에 모듈이름을 명시
print('5초가 지나갔습니다.')
```
한다.

```python
# mylib.py
def add_txt(t1,t2):
    return t1 + ':' + t2

def reverse(x,y,z):
    return z,y,x
```

```python
import mylib

ret1 = mylib.add_txt('대한민국','1등')
ret2 = mylib.reverse(1,2,3)
print(ret1)                     #'대한민국:1등'이 출력됨
print(ret2)                     #(3,2,1)이 출력됨
```