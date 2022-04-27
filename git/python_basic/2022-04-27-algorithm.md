```python
# 정수 N개의 합
# 문제:정수개의 합 - 정수 n개가 주어졌을때 n개의 합을 구하는 함수를 작성하시오

# 작성해야하는 함수는 다음과 같다

# Python 2, Python 3, PyPy, PyPy3: def solve(a: list) -> int
# a: 합을 구해야 하는 정수 n개가 저장되어 있는 리스트 (0 ≤ a[i] ≤ 1,000,000, 1 ≤ n ≤ 3,000,000)
# 리턴값: a에 포함되어 있는 정수 n개의 합 (정수)

def n():
    n = int(input())
    a = type(list(n))
    

    return n

# 정수n개,
# 정수n개의 합을 구하는 리스트 =a
# 리턴값 =리스트에 포함되어 있는 정수 n개의 합..?


```


      File "C:\Users\302-21\AppData\Local\Temp/ipykernel_12976/3898718019.py", line 10
        def a in n
              ^
    SyntaxError: invalid syntax
    



```python
# 정답

def solve(a) : #solve-파이썬 내장함수
    return sum(a) #결과값을 리스트 값으로 변환해서 출력함


#solve 처음 들어보는 함수를 하나 배웠다 
#방정식을 사용할때 사용하는 함수라고한다
```

