```python
#백준알고리즘 1712번 손익분기점

# 노트북 가격이 C만원으로 책정되었다고 한다.
# 일반적으로 생산 대수를 늘려 가다 보면 어느 순간 총 수입(판매비용)이 총 비용(=고정비용+가변비용)보다 많아지게 된다. 
# 최초로 총 수입이 총 비용보다 많아져 이익이 발생하는 지점을 손익분기점(BREAK-EVEN POINT)이라고 한다.
# A, B, C가 주어졌을 때, 손익분기점을 구하는 프로그램을 작성하시오.

#입력:첫째 줄에 A, B, C가 빈 칸을 사이에 두고 순서대로 주어진다. A, B, C는 21억 이하의 자연수이다
#출력:첫 번째 줄에 손익분기점 즉 최초로 이익이 발생하는 판매량을 출력한다. 손익분기점이 존재하지 않으면 -1을 출력한다.

A = int(input()) # 노트북 한대를 생산하는데 사용하는 비용
B  =int(input()) # 가변 비용 
C = int(input()) #손익분기점


#문제 자체를 이해 못하겠음






```

    ljes
    


      File "C:\Users\dladm\AppData\Local\Temp/ipykernel_228/3960323572.py", line 15
        return i
        ^
    SyntaxError: 'return' outside function
    



```python
#정답
A, B, C = map(int, input().split())

if B>=C:
    print(-1)
else:
    print(int(A/(C-B)+1))
    

# 생산하는 대수를 n이라고 하면 A+B*n=C*n일때 수입비용이 같아지기 때문에 
#B>=C일 경우에 손익분기점이 나타나지 않게 되므로 먼저 검사해서 걸러낸다
#생산되는 대수가 늘어날때마다 C와 B의 차이만큼 수입과 비용의 차이가 줄어들게 되므로
#A/(C-B)대 생산했을때 수입과 비용이 같아지기 때문에 +1부터 수입이 많아지게된다

#가면 갈수록 어려워진다... 문제 자체를 이해 못하는 경우도 발생한다.. 
```

    100 70 170
    2
    


```python

```
