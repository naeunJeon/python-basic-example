## 파이썬 패키지 이해하기

```python
import mypackage.mylib          

ret1 = mypackage.mylib.add_txt('대한민국','1등')       #패키지명.모듈명.함수
ret2 = mypackage.mylib.reverse(1,2,3)
```
파이썬 모듈을 계층적인 디렉터리 형태로 구성한 것을 **파이선 패키지**라고 한다. `__init__.py` 라는 이름의 파일이 있어야 한다.<br>
(3.3버전부터는 없어도 패키지로 인식되지만 하위버전과 호환성을 위해 만드는 것이 안전하다.)

### 패키지 만드는 방법
1. mypackage라는 이름의 디렉터리를 만듬
2. mypackage 디렉터리로 이동
3. mylib.py를 mypackage디렉터리로 복사
4. mypackage 폴더에 `__init__.py` 파일을 생성
위 과정을 거치면 mypackage 디렉터리는 하나의 패키지로 구성되고 사용하려면 소스코드 파일이 있는 디렉터리로 mypackage디렉터리 전체를 복사해오면 된다.