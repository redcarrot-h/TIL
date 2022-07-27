## 박스모델 1편, 박스모델 소개

### 박스모델(Box-Model)
브라우저가 요소를 렌더링 할 때, 각각의 요소는 기본적으로 사각형 형태로 영역을 차지하게 된다. 이 영역을 '박스'라 표현하며, CSS는 박스의 크기, 위치, 속성(색, 배경, 테두리 모양 등)을 결정할 수 있다.

하나의 박스는 다음 네 개의 영역으로 구성된다.
- 콘텐츠 영역
- 안쪽 여백
- 경계선(테두리)
- 바깥쪽 여백

### 박스모델(Box-Model)
바깥쪽 여백
	경계선(테두리, border)
		안쪽 여백
			콘텐츠 영역(콘텐츠너비 * 콘텐츠높이)

### 박스 각 영역의 크기는 어떻게?
박스 각 영역의 크기를 정의할 수 있는 속성은 다음과 같다.
 - 콘텐츠 영역 : width, height
 - 안쪽 여백 : padding
 - 바깥쪽 여백 : margin
 - 테두리 : border-width

### 실습
``` css
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            div{ 
                border: 3px solid red;
                padding: 10px; /*안쪽여백*/
                margin: 20px; /*바깥여백*/
                width: 90px;
                height: 35px;
            }
            span{
                width: 100px; height: 100px; 
		/*인라인 요소는 width와 height를 가질 수 없다. display를 inline-block일때만 가능 */
                display: inline-block;
            }
        </style>
    </head>
    <body>
        <div>요소의 콘텐츠</div>
        <span>check</span>
    </body>
</html>
```

출처 : https://www.youtube.com/watch?v=bbeB3Nc5hwY&t=22s
