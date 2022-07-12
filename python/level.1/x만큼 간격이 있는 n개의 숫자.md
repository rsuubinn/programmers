# 📗 x만큼 간격이 있는 n개의 숫자

## 문제 설명

함수 solution은 정수 x와 자연수 n을 입력 받아, x부터 시작해 x씩 증가하는 숫자를 n개 지니는 리스트를 리턴해야 합니다. 다음 제한 조건을 보고, 조건을 만족하는 함수, solution을 완성해주세요.

## 제한 조건

- x는 -10000000 이상, 10000000 이하인 정수입니다.
- n은 1000 이하인 자연수입니다.

## 문제 풀이

```python
def solution(x, n):
    answer = []
    i = 0
    for _ in range(n):
        i += x
        answer.append(i)
    return answer
```

## 알게된 점

- range(_stop_)
- range(_start, stop_)
- range(_start, stop, step_)

이 문제는 한 번에 내 힘으로 해결해서 뿌듯하다 🥺
다른 사람 풀이 보니까 한 줄로 작성하신 분들도 계시는데 정말 대단하다 ...
근데 나도 따라쳐봤는데 문제 해결이 되지는 않음
그러다가 range 함수에 step 인자가 있다는 것을 알게됐다
