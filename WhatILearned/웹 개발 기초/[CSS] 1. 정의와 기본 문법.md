## CSS란? 

### CSS란
CSS는 Cascading Style Sheets를 의미한다.
- Cascading : 계단식
- Style : 멋을 내다
- Sheets : (종이) 한 장

=> 계단식으로 스타일을 정의하는 문서!

CSS는 HTML 문서에 스타일을 더해준다! 
HTML 문서는 태그가 태그를 포함하는 계단식 구조를 지니고 있다.

### CSS가 일하려면
CSS 문서(코드) 자체는 독립적으로 존재할 수 있지만, 그 목적이 구조화된 HTML 뭄ㄴ서의 스타일을 정의하는 데 있으므로 HTML 문서가 없는 CSS 문서는 사실상 의미가 없다.

HTML : 웹 문서의 콘텐츠를 구성하는 언어
CSS : 웹 문서의 콘텐츠에 스타일을 추가하는 언어(색상, 크기, 위미 등)

=> HTML과 함께 사용되지 않은 CSS는 단순 텍스트일 뿐이며, 웹브라우저를 통해 결과물을 확인하기 위해서는 반드시 HTML 문서 작성이 선행되어야 합니다!

출처 : https://www.youtube.com/watch?v=8WruSKR_BK8&t=419s

## CSS 기본 문법 및 사용 방법

### CSS 기본 문법

``` css
선택자{
	속성명: 속성값;
}
```

선택자: 어떤 요소에 스타일을 적용할지에 대한 정보  
{중괄호}: 선택한 요소에 적용할 스타일을 정의하는 영역  
속성명: 어떤 스타일을 정의하고 싶은지에 대한 정보(색상, 크기 등)  
속성값: 어떻게 정의하고 싶은지에 대한 정보

### CSS 기본 문법 사용 예

``` css
p{
	color: red;
}
```
선택자: p 태그에 스타일을 적용하겠다.  
{중괄호}: 이안에 p 태그에 대한 스타일을 정의하겠다.  
속성명: color를 정의하겠다. 이건 글자색을 의미한다.  
속성값: red로 정의하겠다. 빨간색 글자를 원한다.

### 주석
``` css
p{
	/*
	이 안에 작성하면
	주석으로 처리된다
	*/
	/* color: red; */
}
```
주석은 사람에게는 보이지만, 컴퓨터(웹브라우저)에게는 보이지 않는 코드이다.
주로 코드에 대한 메모를 남기기 위한 용도로 사용된다.

### HTML에 CSS를 더하려면
HTML 문서에 CSS 문서(코드)를 적용하고자 할 때는 다음과 같은 방식들을 사용할 수 있다.
- 인라인 스타일 : 태그에 직접 기술하기
- 스타일 태그 : 스타일시트를 위한 태그를 추가하여 기술하기
- 문서간의 연결 : 스타일시트 문서를 따로 작성하여 HTML 문서와 연결하기

### 인라인 스타일
태그에 style 속성을 추가하여 요소에 직접적으로 스타일을 정의하는 방식.  
따라서 선택자는 필요 없다.   
웹 콛텐츠와 스타일시트를 분리하기 위해서는 사용하지 않는 편이 좋다.
``` css
<p style="color: blue;">
	글자를 파랗게 만들어줘
</p>
```
<p style="color: blue;">
	글자를 파랗게 만들어줘
</p>

### 스타일 태그
HTML 문서에 <style></style> 태그를 추가하여 그 안에 CSS 코드를 작성할 수 있다.

``` css
<style>
	/* style 태그 안에는 CSS 코드를 작성해야 한다 */
	p{ color: red;}
</style>
```

### 문서간의 연결
확장자가 *.css인 스타일시트 파일을 생성해 그 안에 CSS 코드를 작성하고, HTML문서에 이를 연결해줄 수 있다. 이떄는 <link> 태그를 사용한다.

``` css
<link href="./style.css" rel="stylesheet">
```

- href: 연결하고자 하는 외부 소스의 url을 기술하는 속성
- rel : 현재 문서(HTML)와 외부 소스의 연관 관계를 기술하는 속성

=> <link> 태그는 HTML 문서의 <head></head> 내부에서 사용해야 합니다!

### 실전 1_ 인라인 방식
``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
    </head>
    <body>
        <p style="color: red;">
            HTML 문서를 준비하고, 에디터로 여신 다음, 내용을 작성하고 브라우저로 확인해주세요.
        </p>
    </body>
</html>
```

### 실전 2_ 스타일 태그
``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            p{
                color: red;
                font-size: 32px;
            }
        </style>
    </head>
    <body>
        <p>
            HTML 문서를 준비하고, 에디터로 여신 다음, 내용을 작성하고 브라우저로 확인해주세요.
        </p>
    </body>
</html>
```

### 실전 3_ 스타일 시트
``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <link href="./style.css" rel="stylesheet">
    </head>
    <body>
        <p>
            HTML 문서를 준비하고, 에디터로 여신 다음, 내용을 작성하고 브라우저로 확인해주세요.
        </p>
    </body>
</html>
```
style.css 
``` css
p{
    color : red;
}
```


출처 : https://www.youtube.com/watch?v=yZq_B6cQ9mo&t=3s