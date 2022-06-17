## 컨테이너 그리고 전역 속성

``` HTML
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>영역을 구분해보자</title>
    </head>
    <body>
    <h1>일단 문서를 만들자</h1>
    <hr>
    <div id="study">        
        <h2 class="title"><span>공부</span> 다짐하기</h2>
        <img src="images/스크린샷 2022-06-02 오후 8.21.51.png" width="300" title="펭귄의 다짐!" alt="펭귄군" />
        <p>펭귄군은 공부를 열심히 하기로 했다!</p>
    </div>
    <hr>
    <div id="workout">
        <h2 class="title"><span>운동</span> 열심히 하기</h2>
        <p>건강을 위해 운동을 열심히 하자!</p>
    </div>
   
    </body>
</html>
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>영역을 구분해보자</title>
    </head>
    <body>
    <h1>일단 문서를 만들자</h1>
    <hr>
    <div id="study">        
        <h2 class="title"><span>공부</span> 다짐하기</h2>
        <img src="images/스크린샷 2022-06-02 오후 8.21.51.png" width="300" title="펭귄의 다짐!" alt="펭귄군" />
        <p>펭귄군은 공부를 열심히 하기로 했다!</p>
    </div>
    <hr>
    <div id="workout">
        <h2 class="title"><span>운동</span> 열심히 하기</h2>
        <p>건강을 위해 운동을 열심히 하자!</p>
    </div>
   
    </body>
</html>


### 컨테이너 태그
콘텐츠나 레이아웃에 아무런 영향도 주지 않고, 단지 다른 요소 여럿을 묶어 관리하게 편하게 만드는 역활을 하는 태그를 '컨테이너'라고 한다.  
콘텐츠 내용을 구분하거나, 공통적인 스타일을 적용하고자 할 때 개발자는 컨테이너를 사용하는 것이 좋다.  
다음 두 가지 태그가 컨테이너 역활을 담당하는 태그들이다.

*div /div : 블록 레벨 컨테이너  
*span /span : 인라인 컨테이너

### 전역 속성
전역 속성(Global attributes)은 모든 HTML 태그에서 공통으로 사용할 수 있는 속성이다.  
속성이란 태그의 부가적인 기능을 정의하는 것으로, 선택사항이다.  
속성은 시작 태그의 내부에 정의한다.  
속성의 개수에는 특별한 제한이 없다.

속성을 추가하는 방법)

``` HTML
<태그명 속성명="속성값" 속성명="속성값">콘텐츠</태그명>
```

### 대표적인 전역 속성들
*id: 요소에 **고유한 이름을 부여**하는 식별자 역할 속성.태그당 하나만 지정.   
*class: 요소를 **그룹 별로 묶을 수 있는** 식별자 역할 속성.다중지정 및 중복 가능.   
*style: 요소에 적용할 CSS 스타일을 선언하는 속성.  
*title: 요소의 추가 정보를 제공하는 텍스트 속성. 사용자에게 툴팁 제공.(커서를 올리면 뜨는 정보)  
 -> 여기서 잠깐! 더 많은 전역 속성에 대한 정보를 알고 싶다면 다음 링크를 참고 하세요:
https://developer.mozilla.org/ko/docs/Web/HTML/Global_attributes

출처 : https://www.youtube.com/watch?v=gC1eEk2O02w