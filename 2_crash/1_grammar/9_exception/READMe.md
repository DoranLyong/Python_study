[(Home)](https://github.com/DoranLyong/Python_study) <br/>
[(back)](https://github.com/DoranLyong/Python_study/tree/master/2_crash/1_grammar)

# 예외 처리 (Exception)
* 코드가 잘못되면 파이썬은 예외(exception)가 발생했음을 알림 
* 이를 처리해 주지 않으면 프로그램이 죽음 
    * ```try ~~ except ~~~ ``` 로 처리해 줌 

    ``` python 
    try:
        """ 코드 표현 """

    except <발생된 예외 메시지>:
        """ 예외 처리 방법 명시 """
    ```

    ``` python 
    try: 
        print(0/0)         # 0으로 나눠서 에러 

    except ZeroDivisionError: 
        print("Cannot divide by zero")
     ```