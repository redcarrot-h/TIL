## select 그리고 textarea

### 보기중에 골라보자
select는 다수의 옵션(선택지)을 포함할 수 있는 선택 메뉴이다. 메뉴 안에 포함되는 옵션은 option 태그를 사용해 표시한다.

### 이름과 값
select에는 input과 마찬가지로 name을 지정할 수 있으며, 각각의 option에는 value 속성을 지정할 수 있다.
value는 실제로 처리될 값을 나타낸다. 

```html
<select name="cafe">
	<option value="starbucks">스타벅스</option>
	<option value="coffeebean">커피빈</option>
	<option value="ediya">이디야</option>
	<option value="pascucci">파스쿠찌</option>
</select>
-> 예를 들어 커피빈을 선택한 경우 'cafe'의 입력값은 'coffeebean'이다.
```

### textarea
textarea는 여러 줄의 일반 텍스트를 입력할 수 있는 입력 요소이다. textarea 역시 name을 추가하여 구별해줄 수 있는 입력 요소이다.

### 실전
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>다양한 입력 요소 만들기</title>
    </head>
    <body>
        <h1>키우고 싶은 동물 고르기</h1>
        <select name="pet" multiple>
            <option value="dog">강아지</option>
            <option value="cat" selected>고양이</option>
            <option value="hamster">햄스터</option>
            <option value="parrot">앵무새</option>
        </select>
        <br>

        <textarea name="content" rows="10" cols="10">기본적으로 쓰여 있는 텍스트</textarea>
    </body>
</html>
```

1. select 태그 안에 multiple이라고 적으면 닫힌 상태가 아닌 펼쳐진 상태에서 모든 value를 볼 수 있으며 ctrl 버튼을 누르면 여러개를 선택할 수 있음.  
2. option 태그 안에 selected라고 적으면 이미 선택이 되어진 상태로 보여짐.  
3. textarea에 rows는 행수, cols는 열수를 지정할 수 있음. 
