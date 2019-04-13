[(Home)](https://github.com/DoranLyong/Python_study)
[(back)](https://github.com/DoranLyong/Python_study/tree/master/2_crash/1_grammar)

# 3rd party packages(제 3자 패키지)
* 제 3자 패키지는 그냥 기본적으로 실행되지 않음 
* 사용하려면 불러올 모듈을 명시해야함 
    ``` python 
    import <모듈 이름> as <별칭>
    import matplotlib.pyplot as plt 
    ```
    * 모듈의 기능(method)나 변수 사용하기 
        * ```<모듈 이름>.<맴버 이름>```
            ``` python 
            import re as regex 
            my_regex = regex.compile( "[0-9]+", regex.I)
            ``` 

<br/>


* 모듈에서 몇몇 특정 기능만 불러오기 
    ```python 
    from keras import modules, layers 
    ```

<br/>

* 가장 안 좋은 습관 
    * 모듈의 기능(method)들을 통째로 불러와 기존의 변수들을 덮어쓰는 것 
    ```python 
    match = 10 

    from re import *     # re 모듈에서 기능들을 다 불러와( * )
    print match          # 이런! re에서 match라는 함수가 존재함 
                         # "<function re.match>"
    ```