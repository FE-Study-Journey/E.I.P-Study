# 🌟 정보처리기사 실기 - Python 정리

## ✅ 가장 중요한 데이터 형

정보처리기사 실기 프로그램에서 Python의 가장 기본적이고 자주 나오는 데이터 형은 다음과 같습니다.

### 1. List (JavaScript의 Array와 비유)

- 다중 항목을 가지고 가능
- 생성, 변경, 제거 가능 (mutable)

```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
print(fruits[1])  # banana
```

- 리스트는 인덱스로 접근 가능하며, `.append()`, `.remove()`, `.insert()` 등 다양한 메서드를 통해 조작 가능

---

### 2. Tuple (JavaScript의 Object.freeze(Array)와 비유)

- 한번 생성하면 변경 불가 (immutable)
- 다중 값 구성, 사용은 list와 비슷하게 가능

```python
tuple_ex = (1, 2, 3)
print(tuple_ex[0])  # 1
```

- 튜플은 리스트처럼 인덱스로 접근 가능하지만, 요소 변경 불가

---

### 3. Set (JavaScript의 Set와 비유)

- 복잡성 없이 고정 인순 없는 값의 무지정 문자 형 집합
- 중복 값은 생렬 후 자동으로 제거됨

```python
unique_nums = {1, 2, 2, 3}
print(unique_nums)  # {1, 2, 3}
```

- 순서가 없고, 인덱싱 불가능

---

### 4. Dictionary (JavaScript의 Object와 비유)

- 키: 값 (문자열이나 정수 등을 키로 사용)
- JSON 같은 것을 보면 이해하기 쉽다

```python
person = {"name": "Tom", "age": 25}
print(person["name"])  # Tom
```

- key를 이용해 직접 접근 가능하며, `.get()` 메서드를 사용해 기본값 처리도 가능

---

## ⚠️ 주의할 것은?

### 1. True / False

- 무조건 대문자로 쓰어야 합니다! (true, false X)
- `True = 1`, `False = 0` 으로 값처럼 사용도 가능

```python
flag = True
if flag:
  print("참입니다")

print(flag + 1)  # 2
```

### 2. slice

- 슬라이싱에서 범위는 `start <= index < end`
- step을 음수로 주면 역순도 가능: `nums[::-1]`

```python
nums = [0, 1, 2, 3, 4, 5]
print(nums[1:5])      # [1, 2, 3, 4]
print(nums[::2])      # [0, 2, 4]
```

- `list[start:end:step]` 형식을 따르며, 특히 `step`의 기본값은 1이고 생략 가능
- `end` 값은 범위에 포함되지 않음

---
