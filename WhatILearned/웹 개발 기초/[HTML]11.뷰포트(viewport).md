## 뷰포트(viewport)

### 뷰포트(viewport)
뷰포트(viewport)란 현재 화면에 보여지고 있는 영역을 의미한다.  
기기 별로 뷰포트가 다르기 때문에, 동일한 웹 페이지라도 기기에 따른 배율 조정이 발생해 화면의 크기가 다르게 보이는 현상이 나타난다.
아래 그림은 동일한 HTML 문서를 각각 PC와 모바일로 확인한 결과이다.

### 왜 이런 현상이?
태블릿, 스마트폰 등 모바일 기기가 등장하기 전에는 웹 페이지가 컴퓨터 화면만을 위해 설계 되었다.  
컴퓨터 화면에서의 웹 페이지는 웹브라우저라는 소프트웨어를 통해 페이지 크기를 조절해가며 웹을 조회할 수 있지만,
모바일 기기에서는 고정된 사이즈(스크린 크기)로 조회해야 하므로 웹의 모든 콘텐츠를 표시하기 위해서는 배율 조정을 해야만 한다. 

=> 때문에 PC용 웹페이지와 모바일 웹페이지를 따로 만드는 경우도 있다!

### name="veiwport"
기기 별로 뷰포트가 다르기 때문에 발생하는 배율 문제에 대응하기 위해 meta 태그를 통해 뷰포트 관련 설정을 추가할 수 있다.

코드 예
``` html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
=> 뷰포트의 너비를 단말기 너비에 맞추고, 초기 배율을 1로 한다!(확대나 축소없이 그대로 보여준다)


### 실전예제
``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta name="viewport"
        content="width=device-width, initial-scale=1.0">
        <title>뷰포트 체험하기</title>
    </head>
    <body>
        <h1>안녕하세요!</h1>
        <h1>감사해요!</h1>
        <h1>잘있어요!</h1>
        <h1>다시만나요!</h1>
    </body>
</html>
```

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta name="viewport"
        content="width=device-width, initial-scale=1.0">
        <title>뷰포트 체험하기</title>
    </head>
    <body>
        <h1>안녕하세요!</h1>
        <h1>감사해요!</h1>
        <h1>잘있어요!</h1>
        <h1>다시만나요!</h1>
    </body>
</html>

출처 : https://www.youtube.com/watch?v=EdFV38Bxm3Y