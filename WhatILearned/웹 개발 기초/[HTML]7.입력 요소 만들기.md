## 입력 요소 만들기

### input
사용자로부터 값을 읿력받을 수 있는 대화형 컨트롤(또는 '필드')을 나타낸다.
기본적으로 인라인 요소이며, 단일 태그이다.


### input의 핵심, type 속성
type의 값에 따라 입력 요소의 형태나 입력 데이터 유형 등이 달라진다. 사용 가능한 type은 20여 가지이며, 기본값은 text이다.
type의 값이 달라짐에 따라 적용할 수 있는 추가 속성의 종류도 조금씩 차이를 보인다.  

  <a href="https://developer.mozilla.org/ko/docs/Web/HTML/Element/Input" target="_black">
https://developer.mozilla.org/ko/docs/Web/HTML/Element/Input</a>

### 이름을 지어주세요
input 태그에는 name 식별자를 추가할 수 있다. 이는 각각의 입력 항목에 대한 이름이다. 
name 속성으로 input 요소를 구별할 수 있다.

```html
<input type="text" name="nickname" />
<input type="text" name="job" />
```
<input type="text" name="nickname" />
<input type="text" name="job" />

-> 입력창에 '유노코딩', '프리랜서'라고 입력한 경우
nickname항목에는 '유노코딩'이, job항목에는 '프리랜서'가 입력된 상태

### 실습하기

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>다양한 입력 요소 만들기</title>
    </head>
    <body>
        <input name="text" type="text" maxlength="5"
        placeholder="메시지 입력..!"/> <br> <br>
        <input name="push" type="button" value="PUSH"/> <br> <br>
        <input name="color" type="color" />색을 골라보세요!<br> <br>
        <input name="score" type="range" max="100" min="0" step="10"/> <br> <br>
        <input name="birthday" type="date" /> <br> <br>
    </body>
</html>
```

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>다양한 입력 요소 만들기</title>
    </head>
    <body>
        <input name="text" type="text" maxlength="5"
        placeholder="메시지 입력..!"/> <br> <br>
        <input name="push" type="button" value="PUSH"/> <br> <br>
        <input name="color" type="color" />색을 골라보세요!<br> <br>
        <input name="score" type="range" max="100" min="0" step="10"/> <br> <br>
        <input name="birthday" type="date" /> <br> <br>
    </body>
</html>