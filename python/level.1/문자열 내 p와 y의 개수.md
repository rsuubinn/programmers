# 📗 문자열 내 p와 y의 개수

## 문제 설명

대문자와 소문자가 섞여있는 문자열 s가 주어집니다. s에 'p'의 개수와 'y'의 개수를 비교해 같으면 True, 다르면 False를 return 하는 solution를 완성하세요. 'p', 'y' 모두 하나도 없는 경우는 항상 True를 리턴합니다. 단, 개수를 비교할 때 대문자와 소문자는 구별하지 않습니다.

예를 들어 s가 "pPoooyY"면 true를 return하고 "Pyy"라면 false를 return합니다.

## 제한사항

- 문자열 s의 길이 : 50 이하의 자연수
- 문자열 s는 알파벳으로만 이루어져 있습니다.

## 문제 풀이

### 내 풀이

```python
def solution(s):
    p_count = 0
    s_count = 0
    for i in list(s):
        if i.lower() == "p":
            p_count += 1
        elif i.lower() == "y":
            s_count += 1
    if p_count == 0 and s_count == 0:
         return True
    else:
        if p_count != s_count:
            return False
        else:
            return True
```

## 알게된 점

### 다른 사람 풀이

```python
def solution(s):
    if s.lower().count("p") == s.lower().count("y"):
        return True
    else:
        return False
```

**count()** : 문자열 안에 인자가 몇 개 있는지 반환하는 함수
