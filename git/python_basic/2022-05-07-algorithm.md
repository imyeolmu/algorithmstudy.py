```python
# 전화를 걸고 싶은 번호가 있다면, 숫자를 하나를 누른 다음에 금속 핀이 있는 곳 까지 시계방향으로 돌려야 한다.
# 숫자를 하나 누르면 다이얼이 처음 위치로 돌아가고, 다음 숫자를 누르려면 다이얼을 처음 위치에서 다시 돌려야 한다.
# 숫자 1을 걸려면 총 2초가 필요하다. 1보다 큰 수를 거는데 걸리는 시간은 이보다 더 걸리며, 한 칸 옆에 있는 숫자를 걸기 위해선 1초씩 더 걸린다.
# 상근이의 할머니는 전화 번호를 각 숫자에 해당하는 문자로 외운다.
# 즉, 어떤 단어를 걸 때, 각 알파벳에 해당하는 숫자를 걸면 된다. 예를 들어, UNUCIC는 868242와 같다.
# 이 전화를 걸기 위해서 필요한 최소 시간을 구하는 프로그램을 작성하시오.알파벳에 해당하는 숫자를 걸면 된다. 
# 예를 들어, UNUCIC는 868242와 같다.

# 입력:첫째 줄에 알파벳 대문자로 이루어진 단어가 주어진다. 
# 단어의 길이는 2보다 크거나 같고, 15보다 작거나 같다.
# 출력:첫째 줄에 다이얼을 걸기 위해서 필요한 최소 시간을 출력한다.
#문자의 길이가 1초



#숫자 하나당 2초가 걸림 -for 문
#그 숫자를 걸기 위해서는 1초가 더 걸림 
#

word = input().split


for i in range(2, 16):
    #숫자와 문자를 어떻게 넣을까,,? 해당하는 문자를 넣어야 되는데
    word[i]+=i #i값을 word의 자릿수로 해야되나,,?
print()
    
    

#솔직히 이문제 어떻게 만들어야 하는지 방향을 못잡겠다
#문자와 숫자를 연결시켜서 그것에 대한 시간을 구해야하는 건데 모르겠음


```

    The Curious Case of Benjamin Button
    


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    ~\AppData\Local\Temp/ipykernel_6700/1484755290.py in <module>
         16 for i in word_list:
         17     cnt_list = word.count(i)
    ---> 18     cnt_list.append(cnt)
         19     print(cnt_list)
         20 
    

    AttributeError: 'int' object has no attribute 'append'



```python
#정답

import sys
input= sys.stdin.readline

Number=['ABC', 'DEP', 'GHI', 'JKL','MNO','PQRS','TUV','WXYZ'] #다이얼 넘버를 받는 NumbeR

li = list((input()) #입력받을 앞바벳
          
# 걸리는 시간
result = 0
          
for i in li:
    for j in Number:
          #입력방은값에 Number에 있으면 index에서 3초를 더해준다
          #1을 선택하면 2초가 걸리고 긔뒤로 갈 수록 1초씩 증가하니 +#3을 인덱스에 해준다
        if i in j:
             result  +=Number.indes(j) + 3
          print(result)
```


      File "C:\Users\dladm\AppData\Local\Temp/ipykernel_10920/3910523898.py", line 11
        result = 0
        ^
    SyntaxError: invalid syntax
    



```python

```
