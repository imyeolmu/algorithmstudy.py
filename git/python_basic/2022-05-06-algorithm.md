```python
# 백준알고리즘 2908번

# 세 자리 수 두 개를 칠판에 써주었다. 그 다음에 크기가 큰 수를 말해보라고 했다.
# 다른 사람과 다르게 거꾸로 읽는다. 예를 들어, 734와 893을 칠판에 적었다면, 
# 상수는 이 수를 437과 398로 읽는다. 따라서, 상수는 두 수중 큰 수인 437을 큰 수라고 말할 것이다.
# 두 수가 주어졌을 때, 상수의 대답을 출력하는 프로그램을 작성하시오.
# 첫째 줄에 상근이가 칠판에 적은 두 수 A와 B가 주어진다. 두 수는 같지 않은 세 자리 수이며, 0이 포함되어 있지 않다.
# 첫째 줄에 상수의 대답을 출력한다.


a= str(input())
b= str(input())

word1=a[::-1]#슬라이드를 이용해서 뒤집은 값 구하기
word2=b[::-1]

if word1>word2:
    print(word1)
else:
        word2<word1
        print(word2)

# 대충 로직을 만들긴했다.. 


```

    734
    893
    437
    


```python
# 정답
num1, num2 = input().split() #split으로 공백을 기준으로 해서 입력받기
num1 = int(num1[::-1])  # [::-1] : 역순
num2 = int(num2[::-1])

if num1 > num2: #변환할 숫자의 크기를 비교한다
    print(num1)
else :
    print(num2)
    
    
#  삼항연산자   print(num1) if num1 > num2 else print(num2) :[ 참일 때 값 if 조건식 else 거짓일 때 값]-조건식이 간단한경우 이런식으로 나타내는 게 좋다

#정답과 거의 80%유사하게 짜긴했는데 아직 미세한 부분을 다루지는 못한다
#다음에는 삼항연산자를 적극 사용해봐야겠다
#그래도 거의 맞아서 뿌듯하다 점차 발전되는거 같다^^
```

    z
    Z
    
