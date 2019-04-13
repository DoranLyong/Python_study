[(Home)](https://github.com/DoranLyong/Python_study) <br/>
[(back)](https://github.com/DoranLyong/Python_study/tree/master/2_crash/1_grammar)

# 코드 블럭 구분자
### 1. 코드 단락 구분하기 
* 중괄호 (curly braces, ```{ }```)
    * C/C++ , Java 
* 들여쓰기 (identation)
    * 공백문자 4칸 or ```[tap]``` 버튼 
    * Python 
    ```python 
    for i in [1, 2, 3, 4]: 
        print i             # "for i" 단락의 첫 번째 줄 
        
        for j in [1, 2, 3, 4]: 
            print j         # "for j" 단락의 첫 번째 줄 
            print i + j     # "for j" 단란의 두 번째 줄 
    print "Finish looping"
    ```


<br/>

### 2. 코드 가독성 높이기  
* 공백문자(whitespace)
    * <b>특징: </b>소괄호(parentheses, ```()```), 대괄호(brackets, ```[]```) 안에서 무시 됨
    * 활용 : 띄어 써서 가독성 높이기 
        ``` python 
        list = [ [1,2,3], [4,5,6], [7,8,9] ]
        ```
* 역슬래시(backslash, ```\```)
    * <b>특징: </b> 코드가 다음 줄로 이어짐 
    * 활용 : 
        ```python 
        add = 2 + \ 
              3 

        add = 2 + 3 

        """ 둘다 같은 코드 """
        ```

<br/>

*** 
<br/>

## 들여쓰기의 문제점 
* 코드를 복사/붙이기 할 때 잘 못 붙어서 에러가 잘 남 
    * ※ IPython에서는 ```%paste``` 라는 명령어를 쓰면 공백문자 & 클립 보드에 있는 무엇이든 제대로 복붙이 됨 