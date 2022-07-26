## 선택자 1편

### 선택자

```css
선택자{
	속성명: 속성값;
}
```

선택자: 어떤 요소에 스타일을 적용 할 것인지에 대한 정보

### 선택자의 종류

- 기본 선택자
- 그룹 선택자
- 특성 선택자
- 결합 선택자
- 의사 클래스
- 의사 요소
 
=> 이번 '선택자 1편에서는 기본 선택자, 그룹 선택자에 대해 알아보겠습니다!

### 기본 선택자 1. 전체 선택자
모든 요소를 선택한다.
*(애스터리스크)는 '문서 내의 모든 요소'를 의미하는 기호이다.

```css
*{
	color: blue;
}
```

=> 문서 내 모든 요소의 글자 색을 파란 색으로 지정한다!

### 기본 선택자 2. 태그 선택자
주어진 이름을 가진 요소를 선택한다. '유형 선택자'라고도 한다.
주어진 이름을 가진 요소가 다수일 경우, 해당 요소들을 모두 선택한다.

``` css
p{
	color: blue;
}
```

=> 문서 내 모든 p 태그 요소의 글자 색을 파란 색으로 지정한다!

### 기본 선택자 3. 클래스 선택자
주어진 class 속성값을 가진 요소를 선택한다.
주어진 class 속성값을 가진 요소가 다수일 경우, 해당 요소를 모두 선택한다.

```css
.text{
	color: blue;
}
```

=> 문서 내 class가 "text"인 모든 요소의 글자 색을 파란 색으로 지정한다!

### 기본 선택자 4. 아이디 선택자
주어진 id 속성값을 가진 요소를 선택한다.
id는 고유한(unique) 식별자 역할을 하는 전역 속성이다.

```css
#topic{
	color: blue;
}
```

=> 문서 내 id가 "topic"인 요소의 글자 색을 파란 색으로 지정한다!

### 그룹 선택자
다양한 유형의 요소를 한꺼번에 선택하고자 할 떄 사용한다.
쉼표(,)를 이용해 선택자를 그룹화한다.

```css
h1, p, div{
	color: blue;
}
```

=> 문서 내 모든 h1, p, div 태그 요소의 글자 색을 파란 색으로 지정한다!


### 선택자가 겹치는 경우
선택자가 겹치는 경우, 기본적으로 나중에 작성된 스타일이 적용된다.  
선택자가 다르지만 요소가 겹치는 경우, 선택자 우선순위에 의해 적용될 스타일이 결정된다.  
선택자 우선순위?  
<strong>아이디 선택자 > 클래스 선택자 > 태그 선택자</strong>

### 실전 예시 1_기본 선택자
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            *{  color: red; }
            h1{ color: blue; }
            p{ color: aqua; }
            .text{ color: olive; } /* 우선순위 : 아이디 선택자 > 클래스 선택자 > 태그 선택자 */
            #gagaga{ color: blueviolet; }
        </style>
    </head>
    <body>
        <h1 class="text">제목을 나타낸다!</h1>
        <p id="gagaga">문단을 표시한다 가가가</p>
        <p class="text">문단을 표시한다 나나나</p>
        <p>문단을 표시한다 다다다</p>
    </body>
</html>
```

### 실전 예시 2_그룹 선택자
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            h1, p {
                color: burlywood;
            }
        </style>
    </head>
    <body>
        <h1 class="text">제목을 나타낸다!</h1>
        <p id="gagaga">문단을 표시한다 가가가</p>
        <p class="text">문단을 표시한다 나나나</p>
        <p>문단을 표시한다 다다다</p>
    </body>
</html>
```

### 실전 예시 3_우선순위
``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>HTML 문서</title>
        <style>
            h1{ color: red;}
            h1{ color: blue;} /* 실행하면 블루로 뜸 */
        </style>
    </head>
    <body>
        <h1 class="text">제목을 나타낸다!</h1>
        <p id="gagaga">문단을 표시한다 가가가</p>
        <p class="text">문단을 표시한다 나나나</p>
        <p>문단을 표시한다 다다다</p>
    </body>
</html>
```



출처 : youtube.com/watch?v=ZDNHpONynUk&t=60s