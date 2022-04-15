```python
# 백준 알고리즘
# 문제:두 정수 A와 B를 입력받은 다음, A+B를 출력하는 프로그램을 작성하시오.
#입력: 첫째 줄에 테스트 케이스의 개수 T가 주어진다.각 테스트 케이스는 한 줄로 이루어져 있으며, 각 줄에 A와 B가 주어진다. (0 < A, B < 10)
#출력:각 테스트 케이스마다 "Case #x: "를 출력한 다음, A+B를 출력한다. 테스트 케이스 번호는 1부터 시작한다.

t= int(input())
a= int(input())
b= int(input())

for i in range(1,t):
    print(CASE # a :a+b)
    

```


      File "C:\Users\302-21\AppData\Local\Temp/ipykernel_2216/1773734590.py", line 12
        
        ^
    SyntaxError: unexpected EOF while parsing
    



```python
# 정답

num = int(input()) 
for i in range(num):
    a, b = map(int, input().split())
    print("Case #%d: %d" %(i+1, a+b))
#T를 입력받고 T개의 정수쌍을 입력받은후 각줄마다 Case #xA+B를 출력하면된다
#처음 접해보는 CASE를 이용한 문제가 조금 약한거 같다,, 

```
