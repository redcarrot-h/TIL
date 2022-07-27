## 박스모델 2편, margin padding 다루기

### padding 과 margin 

magin : 테두리(border) 바깥쪽 여백
padding : 테두리(border)와 콘텐츠 영역의 사이 여백

### 다양한 경우의 수
여백은 상하좌우 네 개의 면에 존재하는 영역이다.
작성자는 각 면에 개별적으로 두께를 정의할 수 있다.
이를 위해 다음 두 가지 방법을 사용한다.

- 하위 속성 정의하기
- 여러 값을 한 번에 정의하기

### 하위 속성 정의하기
상하좌우 여백을 정의할 수 있는 개별 속성들이 있다?!  
padding-left padding-top padding-right padding-bottom  
=> margin에도 동일한 접미사를 붙여 개별 정의할 수 있습니다.

### 여러 값을 한 번에 정의하기 
padding과 margin은 네 면의 여백에 대한 단축속성이다.

``` css
span{
	display: inline-block;
	width: 100px; height: 100px;
	margin: 10px 20px 30px 40px; /*위, 오른쪽, 아래, 왼쪽 */
}
```

### 실습
``` css
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            div{
                width: 100px; height: 100px;
                border: 5px solid red;
                margin: 10px 30px 20px 40px; 
		/* 2개 수치는 위아래, 좌우 여백, 3개 수치는 위, 좌우, 아래 여백, 4개 수치는 위, 오른쪽, 아래, 왼쪽 */
            }
        </style>
    </head>
    <body>
        <div></div>
    </body>
</html>
```


출처 : https://www.youtube.com/watch?v=NtQeb-cpNMg&t=24s
