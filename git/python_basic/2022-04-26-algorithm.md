```python
# 백준알고리즘 4344번
# 대학생 새내기들의 90%는 자신이 반에서 평균은 넘는다고 생각한다. 당신은 그들에게 슬픈 진실을 알려줘야 한다.

# 첫째 줄에는 테스트 케이스의 개수 C가 주어진다.
# 둘째 줄부터 각 테스트 케이스마다 학생의 수 N(1 ≤ N ≤ 1000, N은 정수)이 첫 수로 주어지고, 
# 이어서 N명의 점수가 주어진다. 점수는 0보다 크거나 같고, 100보다 작거나 같은 정수이다.
# 각 케이스마다 한 줄씩 평균을 넘는 학생들의 비율을 반올림하여 소수점 셋째 자리까지 출력한다.

t = int(input())


for n int(range(t)):
    for  m  range((n)):            #테스트 케이스마다 학생수를 받기
        m = list(int, input().split())  #학생 점수 받기
        sum += m[n]                     #점수를 게속 더하기
print('%3f',sum/n)                        #학생점수 평균내서 반올림하여 셋쨰자리까지 출력하기
    
# 음 나름 생각을 했는데  틀렸다^^



```


      File "C:\Users\302-21\AppData\Local\Temp/ipykernel_8300/2486847016.py", line 12
        for n int(range(t)):
              ^
    SyntaxError: invalid syntax
    



```python
# 정답:

t= int(input())
    
for i in range(t): #테스트 케이스마다 학생수 받기
    li = list(map(int, input().split())) #학생점수 리스트형태로 받기
    t=0
    for j in li[1:]: # 리스트 첫번째부터 끝까지 돌리기
        avg = sum(li[li:])/li[0] #리스트를 더하면서 평균을 구한다
        if j >avg:
            t+=1  #
        rate=t/li[0]*100#평균을 넘는 학생들의 비율을 구한다
        print('{0:0.3f}%'.format(rate)) #format함수 사용하기-{}안에 출력할 형식을 지정하고 format에 값을 넣어준다
    
    
    
  # 파이썬을 공부하면서 다 배웠던것들인데 어떻게 쓰는지를 잘 모르겠다
    #눈에 익히는 연습을 해야할거같다



```

    5
    5
    50 50 70 80 100
    


    

