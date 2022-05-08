```python
# 예전에는 운영체제에서 크로아티아 알파벳을 입력할 수가 없었다. 따라서, 다음과 같이 크로아티아 알파벳을 변경해서 입력했다.
# ljes=njak은 크로아티아 알파벳 6개(lj, e, š, nj, a, k)로 이루어져 있다. 단어가 주어졌을 때, 
# 몇 개의 크로아티아 알파벳으로 이루어져 있는지 출력한다.
# dž는 무조건 하나의 알파벳으로 쓰이고, d와 ž가 분리된 것으로 보지 않는다. lj와 nj도 마찬가지이다. 위 목록에 없는 알파벳은 한 글자씩 센다.

words = ['c=', 'c-', 'dz=', 'd-', 'lj', 'nj', 's=', 'z=']
word= list(input())

for  i in word:
    for j  in words:
        if i in j:
            word[i]== words[j]
            print(len(word))
        else:
            return i
     #word의 길이를 출력하는거,,, len 함수를 이요하고 
    #변수랑 변수를 이어야하는데 모름...

```

    ljes
    


      File "C:\Users\dladm\AppData\Local\Temp/ipykernel_228/3960323572.py", line 15
        return i
        ^
    SyntaxError: 'return' outside function
    



```python
#정답
croatia = ['c=', 'c-', 'dz=', 'd-', 'lj', 'nj', 's=', 'z=']
word = input()

for i in croatia : #croatia을 돌리면서 word와 같은 것을 
    word = word.replace(i, '*')  # input 변수와 동일한 이름의 변수
print(word)#동일한 문자가 있으면 *으로 출력된다
print(len(word))
#문자를 변환하는 함수인 replace함수는 문자열 변형을 시키지 않는 비파괴적인 함수 이다

#replace 함수를 배운거 같은데 기억이 안난다 계속 쓰지를 않으니 까먹는거 같다
#복습복습이 살길이다 알고리즘을 공부하면서 함수를 여러방면으로 사용할 수 있어서 
#사고력이 점차 늘어나는거 같다 꾸준히 하다보면 답이 나오겠지!
```

    ljes=njak
    *e**ak
    6
    


```python

```
