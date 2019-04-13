[(Home)](https://github.com/DoranLyong/Python_study) <br/>
[(back)](https://github.com/DoranLyong/Python_study/tree/master/2_crash/1_grammar)

# Function (함수)
### 입력받은 인자들(factors)에 대한 인과관계를 처리하고 결과를 출력하는 '<span style="color:skyblue">규칙 박스</span>'
> input → [함 수] → output  


* 입력 받는 인자 개수: 
    * 0 ~ n 개 
* 출력 개수 :  
    * 0 ~ n 개 

<br/>

## 1. 정의 방법 
```python 
def <함수 이름>(parameters):
    """ 규칙 기술 """ 

    return x * 2 
```

<br/>

## 2. 일등 시민 함수(first-class)
* 파이썬 함수는 변수로 할당되거나 함수의 인자로 전달 될 수 있음 
    * ```함수_이름``` ⇒ 객체로 취급 
    * ```함수_이름( )``` ⇒ 함수 실행 

        ``` python 
        def func(x):
            print(x)

        def apply_to_one(func):  # 함수를 함수의 인자로 전달 
            func(1)

        sample = func            # 함수를 변수에 할당 
        sample(2)                # 함수 복사됨 
        >> 2 
        ```

<br/>

## 3. 파이썬스러운 함수 정의 
* 람다 함수(lambda fucntion)