### 목록
목록은 연관 있는 항목(item)들을 나열한 것으로 의미한다.
HTML 목록은 '순서 없는 목록'과 '순서 있는 목록'으로 구분된다.

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>목록 만들기</title>
    </head>
    <body>
        <h1>귀여운 동물 목록</h1>
        <ul>
            <li>강아지</li>
            <li><strong>고양이</strong></li>
            <li>두더지</li>
            <li>햄스터</li>
        </ul>
        <hr>
        <h1>프로그래밍 공부 순서</h1>
        <ol>
            <li><mark>HTML</mark></li>
            <li>CSS</li>
            <li>JAVASCRIPT</li>
            <li>NODEJS</li>
        </ol>
    </body>
</html>
```

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>목록 만들기</title>
    </head>
    <body>
        <h1>귀여운 동물 목록</h1>
        <ul>
            <li>강아지</li>
            <li><strong>고양이</strong></li>
            <li>두더지</li>
            <li>햄스터</li>
        </ul>
        <hr>
        <h1>프로그래밍 공부 순서</h1>
        <ol>
            <li><mark>HTML</mark></li>
            <li>CSS</li>
            <li>JAVASCRIPT</li>
            <li>NODEJS</li>
        </ol>
    </body>
</html>

<hr>

Unordered List(ul/ul)
* 토끼
* 다람쥐
* 청설모
* 호랑이  

Ordered List(ol/ol)
1. HTML
2. CSS
3. JavaScript  

### 항목 태그는 같은 것을 쓴다
li 태그는 목록에 들어가는 항목 하나 하나를 표현할 때 사용하는 태그이다.
항목들(li 태그들)을 감싸는 태그가 무엇이냐에 따라 기호가 달라진다.

```html
<ul>
	<li>토끼</li>
	<li>다람쥐</li>
	<li>청설모</li>
	<li>호랑이</li>
</ul>

<ol>
	<li>HTML</li>
	<li>CSS</li>
	<li>JavaScript</li>
</ol>
```
<ul>
	<li>토끼</li>
	<li>다람쥐</li>
	<li>청설모</li>
	<li>호랑이</li>
</ul>

<ol>
	<li>HTML</li>
	<li>CSS</li>
	<li>JavaScript</li>
</ol>

-> ul, ol, li는 모두 블록 레벨 요소를 만드는 태그이다!

출처 : https://www.youtube.com/watch?v=sp4ruWfpY2k&list=PLFeNz2ojQZjtQc7mt8E9fNzIh9or34A61&index=11
