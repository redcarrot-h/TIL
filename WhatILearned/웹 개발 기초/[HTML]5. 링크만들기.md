## 링크 만들기

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>링크 만들기</title>
    </head>
    <body>
        <a href="https://www.naver.com" target="_self">
            네이버로 갑시다!
        </a>
        <br>
        <a href="https://www.google.com" target="_black">
            구글로 갑시다!
        </a>
        <br><br>

        <a href="tel:010-1234-5678">010-1234-5678</a>
        <br>
        <a href="mailto:abc@naver.com">
            abc@naver.com
        </a>
    </body>
</html>
```

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>링크 만들기</title>
    </head>
    <body>
        <a href="https://www.naver.com" target="_self">
            네이버로 갑시다!
        </a>
        <br>
        <a href="https://www.google.com" target="_black">
            구글로 갑시다!
        </a>
        <br><br>

        <a href="tel:010-1234-5678">010-1234-5678</a>
        <br>
        <a href="mailto:abc@naver.com">
            abc@naver.com
        </a>
    </body>
</html>


### 링크는 anchor
a 태그 요소는 href 속성을 통해 다른 페이지, 전화번호, 이메일 주소와 그 외 다른 url로 연결할 수 있는 링크(연결)를 만든다.  
인라인 요소이며, 콘텐츠는 주로 링크의 목적지를 나타낸다.

### 새 탭에서 열고 싶다
a 태그의 target 속성을 이용하면 새로운 문서를 열 때 현재 탭에서 열지, 새로운 탭에서 열지 결정할 수 있다.
```html
<a href="https://www.naver.com" target="_self">
	현재 탭에서 열기(기본값)
</a>

<a href="https://www.naver.com" target="_black">
	새 탭에서 열기
</a>
```

### 연락을 해보자
a 태그의 href에는 웹문서의 주소 뿐 아니라 전화번호나 메일 주소 등을 지정할 수도 있다.  
이때 각 유형별로 추가되는 텍스트가 있다.

```html
<a href="tel:010-1234-5678" target="_self">
	전화 걸기
</a>

<a href="mailto:beansdrawer@naver.com" target="_blank">
	메일 쓰기
</a>
```