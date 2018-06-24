#튜플 이해하기(())

```python
tuple1 = (1,2,3,4,5)
tuple2 = ('a','b','c')
tuple3 = (1, 'a', 'abc', [1,2,3,4,5], ['a','b','c'])
```
튜플은 리스트와 비슷한 자료형으로 임의의 객체를 요소로 가질 수 있지만 요소의 값을 변경할 수 없다는 특징이 있다.
```python
tuple1[0] = 6
```
tuple1[0]의 값을 6으로 변경하려면 아래와 같은 오류가 발생한다. <br>
**TypeError:'tuple' object does not support item assignment**

```python
def myfunc():
    print('안녕하세요')
tuple4 = [1, 2, myfunc];
tuple4[2]()                 #'안녕하세요'가 출력됨
```