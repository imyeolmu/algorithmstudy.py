```python
# 백준알고리즘 1316번 
#그룹단어체커

# ccazzzzbb는 c, a, z, b가 모두 연속해서 나타나고, kin도 k, i, n이 연속해서 나타나기 때문에 그룹 단어이지만,
# aabbbccb는 b가 떨어져서 나타나기 때문에 그룹 단어가 아니다.
# 단어 N개를 입력으로 받아 그룹 단어의 개수를 출력하는 프로그램을 작성하시오.
# 첫째 줄에 단어의 개수 N이 들어온다. N은 100보다 작거나 같은 자연수이다. 둘째 줄부터 N개의 줄에 단어가 들어온다.
# 입력:단어는 알파벳 소문자로만 되어있고 중복되지 않으며, 길이는 최대 100이다.
# 출력:첫째 줄에 그룹 단어의 개수를 출력한다.



n = int(input())
word = []
for  i in range(n):
    word= list(set(input())
               
    print (len(word))
    
   
#중복된 값을 제거 해줘야하는데 set을 써줘야하는건가


```


      File "C:\Users\302-21\AppData\Local\Temp/ipykernel_3468/3087816539.py", line 18
        print (len(word))
        ^
    SyntaxError: invalid syntax
    



```python
# 정답
n = int(input())

group_word = 0 #그룹단어의 개수를 저장할 변수를 group_word를 생성해서 0을 선언
for _ in range(n): #맨 처음 단어의 개수 n개를 입력받으면 for문을 n번 반복한다  
    word = input() #for 문을 반복하는 동안  word에 변수를 선언한다
    error = 0 #error은 그룹단어가 아닌경우를 찾는데 사용한다
    
    for index in range(len(word)-1): #range함수로 입력 받는 단어의 개수보다 1개 적은 숫자의 범위를 생성(0부터 단어개수-1까지)하고 아래 index로 받음
        if word[index] != word[index+1]: #두 알파벳을 비교해서 두알파벳이 다른경우 남은 경우 남은 문자열 생성
            new_word = word[index+1:]#현재 글자 이후 문자열을 새로운 단어로 생성한다
            if  new_word.count(word[index])>0: # count함수로 동일한 알파벳이 있는지 확인한다
                               error +=1 #반환된 함수가 0이 아닌경우 그룹단어가 아니므로 변수에 1을 더해준다
                               
    if error ==0:   
        group_word +=1 #error 변수가 0이면 그룹단어이므로 if 조건식을 이용해서 error변수가 0인경우 group_word 변수의 숫자를 1 더한다
print(group_word)  
    
    
    
#전체적인 문제는 이해 갔는데 너무 어렵다... 정답코드도 거의 이해를 못하겠다  
#알파벳을 하나하나 확인해서 옆과 비교를 해야해야되고 그것들이 다른 동일한 알파벳이 있는지 확인을 해줘야 하는.... 어려운 문제였다
#리스트를 사용해서 하는건지 정규식? 그것도 찾아봤다... 중복된 변수를 제거하는거에만 초점을 맞췄는데 옆옆과도 계속 비교를 해줘야되고
#하나하나씩 비교를 해야되었다 그래도 60퍼센트는 이해를 한거 같긴하다... 열심히 해야지!!
```

    3
    happy
    new
    year
    3
    
