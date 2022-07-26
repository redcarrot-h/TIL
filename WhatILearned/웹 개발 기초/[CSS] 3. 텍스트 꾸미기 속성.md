## 텍스트 꾸미기 속성

### 함께 공부해 볼 텍스트 관련 속성
- font-family: 글꼴을 정의한다.
- font-size: 글자 크기를 정의한다.
- text-align: 정렬 방식을 정의한다.
- color: 글자 색상을 정의한다.

### font-family
요소를 구성하는 텍스트의 글꼴을 정의한다. 글꼴명을 속성값으로 지정한다. 여러 개의 글꼴을 연달아 기입하여 우선 순위를 지정할 수 있다.

사용 예
``` css
*{
	font-family: Times, monospace, serif;
}
```
=> Times를 우선 지정하되, 지원되지 않을 경우 monospace를 지정한다!

### 실전 예제
``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            *{ font-family: 굴림, serif, monospace;} /*굴림체가 없으니 serif로 지정됨*/
        </style>
    </head>
    <body>
        <h1>아무 내용</h1>
        <p>하하 반가워요~!^^</p>
    </body>
</html>
```

### font-size
수치와 단위를 지정해 글자의 크기를 정의할 수 있다.

| 단위 | 의미 |
|:----------|:----------|
| px   | 모니터 상의 화소 하나 크기에 대응하는 절대적인 크기  |
| rem  | <html> 태그의 font-size에 대응하는 상대적인 크기   |
| em   | 부모태그(상위태그)의 font-size에 대응하는 상대적인 크기   |

사용 예
```css
span{ font-size: 16px; }
span{ font-size: 2rem; }
span{ font-size: 1.5em; }
```

### 실전 예제
``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            html{ font-size: 18px; }
            h1{font-size: 2rem; }
            p{font-size: 16px; } 
            span{ font-size: 5em; }
            /*원래 h1은 32px, p는 16px임, 
            rem은 html의 px의 배수만큼 크기를 조정한다. 
            span태그는 p태그의 하위태그이기때문에 span태그는 5*16 = 80px로 보인다. */
        </style>
    </head>
    <body>
        <h1>아무 내용</h1>
        <p>하하 반가워요~!^^<span>호호</span></p>
    </body>
</html>
```

### text-align
블록 내에서 텍스트의 정렬 방식을 정의한다. 미리 정의된 키워드 값을 지정한다.

| 속성값  | 의미  |
|:----------|:----------|
| left / right    | 왼쪽 또는 오른쪽 정렬한다.    |
| center    | 가운데 정렬한다    |
| justify    | 양끝 정렬한다(마지막 줄 제외)    |

사용 예
``` css
p{ text-algin: right; }
```

### color
텍스트의 색상을 정의한다. 다양한 방법으로 색상을 지정할 수 있다.

| 속성값 유형  | 방법  |
|:----------|:----------|
| 키워드    |  미리 정의된 색상별 키워드를 사용한다.(ex. red, blue)    |
| RGB 색상 코드    | # + 여섯자리 16진수 값 형태로 지정한다.    |
| RGB 함수    | Red, Green, Blue의 수준을 각각 정의해 지정한다.    |

사용 예
``` css
span{ color: red; }
span{ color: #FF0000; }
span{ color: rgb(100%, 0%, 0%); }
```
=> 놀랍게도, 모두 같은 색입니다!

### RGB, 그게 뭔데!?
RGB 색상은 빛의 삼원색(Red, Green, Blue)을 혼합하여 색을 정의하는 방식이다. 모든 수치가 가장 높을 때 흰색이 된다.

``` css
/* R:00, G:00, B:00 */
span{ color: #000000; }
/* R: 70%, G: 10%, B: 20% */
span{ color: rgb(70%, 10%, 20%); }
```



출처 : youtube.com/watch?v=tvMxptAqWSI&t=2s