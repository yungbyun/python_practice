## My Python practice page

> 사실 복잡한데, 그냥 간단히 줄여서 표현하는 거 – Abstraction 추상화 -> 뭐를 추상화? 코드를 추상화 -> 코드 추상화 -> 하면 무엇이 만들어지> 나? 함수라고 한다.

```
def show_msg():
    print('Hello,World!')
    print('Hello,World!')
    print('Hello,World!')
    print('Hello,World!')
    print('Hello,World!')
    print('Hello,World!')

show_msg()
print('The End!')
```

파이썬에서는 변수를 언제 만들까? [정답] 값을 할당할 때

def add():
    return a + b
    
a = 2 //여기 (전역변수)
b = 3 //여기 (전역변수)

c = add() //여기

print(c)


-----

def add():
    return a + b

def assign():
    a = 2
    b = 3

a = 0
b = 0

assign()

c = add()

print(c)


-----

def add():
    return a + b


def assign():
    global a, b
    a = 2
    b = 3


a = 0
b = 0

assign()

c = add()

print(c)

----
XXX를 자료형

묶자 XXX 시작
def add(): 
    imsi = a + b
    return imsi

def assign():
    global a, b
    a = 2
    b = 3

a = 0  
b = 0  
끝

assign()

c = add()

print(c)


Python vs C 

C언어에서는 
integer <- 정수(자료형)라는 단어

int a = 0;
int b = 0;

char d = ‘A’;

int a, b, c; //int라는 자료형으로 변수 3개 만들고 있음. int라는 부류에 속하는 변수들 a, b, c
깡패 gildong, cheolsu, youngja; //깡패라는 부류에 속하는 길동, 철수, 영자

자료형은 변수만들라고 있는거여...


-----
XXX를 자료형(int, char)이라고 한다.
아빠, 그럼 우리가 자료형을 만들 수도 있어요?
그럼...
자료형은 뭐하라고 있는거지? 변수만들라고 있는거...
int. a, b, c;
XXX a, b, c;
깡패 gildong, cheolsu, youngja;
gildong = 깡패()

묶자 깡패 시작
def add(): 
    imsi = a + b
    return imsi

def assign():
    global a, b
    a = 2
    b = 3

a = 0  
b = 0  
끝

assign()

c = add()

print(c)



----

class XXX:  # gildong
    def add(self):
        imsi = a + b
        return imsi

    def assign(self, i, j):
        global a, b
        a = i
        b = j

    a = 0
    b = 0


gildong = XXX()

gildong.assign(7, 8)
c = gildong.add()
print(c)

이제까지는 bottom-up
그렇다면 Top-down 방식은 어떻게?

----

class Car:
    def turnLeft(self, i):
        print('turn Left')

    def turnRight(self, j):
        print('turn right')

    def stop(self):
        print('stop')

    def start(self):
        print('start')

    def goBack(self):
        print('go back')


myCar = Car()
myCar.turnLeft(10)
myCar.turnRight(5)
myCar.stop()
myCar.start()
myCar.goBack()


-----

yeseo = MoviePlayer()
yeseo.play("permission to dance.mp4")
