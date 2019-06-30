---
-layout: post
-title: 파이썬(Python)에서 JSON 사용하기
-date:  2019-06-30 17:43:00 +0900
-categories: blog
---

# 파이썬(Python)에서 JSON 사용하기

## Encode

파이썬에서 Object(개체)를 JSON으로 인코딩(Encoding)하기 위해서는 다음과 같이 작성한다. 
 
 코드
```python
  1 import json
  2
  3 obj = {
  4   "name": "Jaeryol",
  5   "favorite_sports": [
  6         "soccer",
  7         "baseball",
  8         "swimming"
  9    ]
 10 }
 11
 12 print(obj)
 13 print(f"타입 : {type(obj)}")
 14 print()
 15
 16 print("After encoding------")
 17 print()
 18
 19 encoding = json.dumps(obj)
 20 print(encoding)
 21 print(f"타입 : {type(encoding)}")
```

실행 결과
```
➜ python json_encode.py
{'name': 'Jaeryol', 'favorite_sports': ['soccer', 'baseball', 'swimming']}
타입 : <class 'dict'>

After encoding------

{"name": "Jaeryol", "favorite_sports": ["soccer", "baseball", "swimming"]}
타입 : <class 'str'>
```
json으로 인코딩 후 결과를 확인해보면 타입이 `dic`에서 `str`로 변경된 것도 확인할 수 있다.


## Decode
JSON을 디코딩(Decoding)하기 위해서는 다음과 같이 작성한다.

코드
```python
  1 import json
  2
  3 jsonString = '{"name": "Jaeryol", "favorite_sports": ["soccer", "baseball", "swimming"]}'
  4 print(jsonString)
  5 print(f"타입 : {type(jsonString)}")
  6 print()
  7
  8 print("After decoding-----------")
  9 print()
 10
 11 obj = json.loads(jsonString)
 12 print(obj)
 13 print(f"타입 : {type(obj)}")

```

실행 결과
```
➜ python json_decode.py
{"name": "Jaeryol", "favorite_sports": ["soccer", "baseball", "swimming"]}
타입 : <class 'str'>

After decoding-----------

{'name': 'Jaeryol', 'favorite_sports': ['soccer', 'baseball', 'swimming']}
타입 : <class 'dict'>
```
json을 디코딩 후 결과를 확인해보면 타입이 `str`에서 `dic`으로 변경된 것도 확인할 수 있다.