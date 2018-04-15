## 1.시퀀스 자료형 이해하기

시쿼스 자료형은 어떤 객체가 순서를 가지고 나열되는 것이다.

```python
strdata = 'abcde'
listdata = [1,[2,3],'test']
tupledata = (1,2,3)
```
**문자열, 리스트, 튜플**은 시퀀스 자료형에 해당한다.

또한 이 시퀀스 자료형은 다음과 같은 공통점이 있다.

1.인덱싱(인덱스를 통해 값에 접근할 수 있음)<br>
2.슬라이싱(특정구간의 값을 취할 수 있음)<br>
3.연결('+'로 시퀀스 자료를 연결 할 수 있음)<br>
4,반복('*'로 시퀀스 자료를 반복 할 수 있음)<br>
5,멤버체크('in'키워드로 특정 값이 시퀀스 자료에 포함되어 있는지 확인할 수 있음)<br>
6,크기정보('len()'로 시컨스 자료의 크기를 알 수 있음)