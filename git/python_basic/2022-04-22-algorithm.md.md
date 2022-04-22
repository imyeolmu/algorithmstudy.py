```python
# 세 개의 자연수 A, B, C가 주어질 때 A × B × C를 계산한 결과에 
# 0부터 9까지 각각의 숫자가 몇 번씩 쓰였는지를 구하는 프로그램을 작성하시오.
# 예를 들어 A = 150, B = 266, C = 427 이라면 A × B × C = 150 × 266 × 427 = 17037300 이 되고,
# 계산한 결과 17037300 에는 0이 3번, 1이 1번, 3이 2번, 7이 2번 쓰였다.


a=int(input())
b=int(input())
c=int(input())



i = a*b*c

for n in range(10): #0부터 9까지의 숫자
    i_list = list(map(int, str(i)))# 곱한값을 list형으로 변환
    print(i.conut(n))#카운트로 n의 값을 돌린다
    
#     곱하고 리스트 형태로 변환?하기 
    
    

```

    150
    266
    427
    


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    ~\AppData\Local\Temp/ipykernel_9232/1680015779.py in <module>
         15 for n in range(10): #0부터 9까지의 숫자
         16     i_list = list(map(int, str(i)))# 곱한값을 list형으로 변환
    ---> 17     print(i.conut(n))#카운트로 n의 값을 돌린다
         18 
         19 #     곱하고 리스트 형태로 변환?하기
    

    AttributeError: 'int' object has no attribute 'conut'



```python
#정답

a = int(input())
b = int(input())
c = int(input())

result = list(str(a * b * c)) #리스트 자체에 넣어도됨!
for i in range(10):
    print(result.count(str(i)))
    
#얼추 비슷하게 풀은거같은데 아직 인수를 넣는 사고가 부족한거같다
#어제보다 문제 파악하는 시간을 더욱 가졌다 - 빠르게 풀 생각하지말고 차분하게 파악해야겠다
#그래도 차근차근 사고력이 괜찮아지는것 같다 아직 멀었긴하지만 계속 도전해야겠다
```

    3 
    29
    38
    12
    57
    74
    40
    85
    61
    85
    8
    
