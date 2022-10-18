# 파이썬 알고리즘 문제풀이를 위한 CheetSheet

- 파이썬언어로 알고리즘 문제를 풀 때, 기억나지 않는 것을 빠르게 보기 위해 만들었습니다.

- [문자열](#문자열)
- [정규표현식](#정규표현식)
- [딕셔너리](#딕셔너리)
- [클래스](#클래스)
- [복사](#복사)
- [배열](#배열)
- [반복문](#반복문)
- [정렬](#정렬)

---------------------------------------------------------


## 문자열

### 자료구조 (Trie)
- https://blog.ilkyu.kr/entry/%ED%8C%8C%EC%9D%B4%EC%8D%AC%EC%97%90%EC%84%9C-Trie-%ED%8A%B8%EB%9D%BC%EC%9D%B4-%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0
- 접두사를 통해 빠르게 문자열 검색을 할 수 있다.
- 2020 카카오 신입공채 문제


## 정규표현식

- 정규표현식 테스트 사이트 https://regexr.com/
- 참고 사이트 https://wikidocs.net/4308#finditer


* re 모듈 import

```python

import re
p = re.compile('ab*')

```

1. match()

```python

m = p.match("python")

```
- 문자열의 처음부터 매치, 매치되면 match 객체 리턴 아니면 None

2. search()

- match 와 비슷하나 문자열 전체에서 검색

3. findall()

- 매치되는 모든 문자열을 띄어쓰기로 구분하여 리턴 (배열로 리턴)

4. finditer()

- findall 과 비슷하지만 반복가능한 객체로 리턴해줌.


## 딕셔너리

- https://wikidocs.net/16#key-valueget


## 클래스

- https://wikidocs.net/28

## 복사

- 리스트의 copy https://wikidocs.net/16038
- 그냥 변수에 넣어주다가 낭패봄..
- 확실히 이것으로 복사해주는게 나을 듯 합니다.

```python

import copy
b = copy.deepcopy(a)

```

## 배열

-  배열 초기화

```python

# 1차원 배열
arr = [0 for _ in range(2)]

# 2차원 배열
import numpy as np

a = np.zeros((2,2), dtype=int)

# https://076923.github.io/posts/Python-numpy-3/
# [[0 0]
# [0 0]] 로 출력

```


## 반복문

1. for-else 문
- http://www.mukgee.com/?p=93
- for문이 완전히 잘 끝나면, else 문을 실행

```python

for a in arr:
    print(a)
else:
    print('else')
    
```

2. range
- https://codechacha.com/ko/python-range/

```python

range(start, stop, step)
# ex) 하나씩 작아지는 range
# range(10, -1, -1)

# list()로 range를 list로 반환도 가능
result = list(range(1, 10, 2))
print(result)
# [1, 3, 5, 7, 9]
```


## 정렬

1. sort
- https://docs.python.org/ko/3/howto/sorting.html
```python


```
