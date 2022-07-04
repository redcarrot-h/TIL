## 폼(form) Part1. 서버와 클라이언트

### form을 학습하기 전에
form은 사용자가 입력한 데이터(입력값)를 서버로 보내기 위해 사용하는 태그
서버란, 정보를 제공하는 호스트(host)이다.

### 서버와 클라이언트
클라이언트(사용자)가 요청을 하면, 서버는 그에 대한 응답으로 정보를 제공한다.   
클라이언트가 어떤 요청을 보내는가에 따라, 응답은 달라질 수 있다.  
 -> 로그인 양식은 세 개의 입력 요소로 구성되어 있으며, 세 개의 입력 데이터는 form을 통해 서버로 전송된다!

## 폼(form) Part2. 폼 태그

### form
form은 입력 요소들을 감싸며, 입력 값을 서버 측으로 제출(submit)할 수 있다.

### form의 내용을 제출
form의 내용(입력값)을 제출하기 위해 input 태그의 submit 타입 사용 가능!  
-> '로그인'버튼을 누르면 입력된 아이디와 비밀번호가 서버로 전송되고(요청), 서버 측에서 데이터를 처리한 결과를 클라이언트에게 보내준다(응답).

### form의 속성
action: 입력값을 전송할 서버의 url
method: 클라이언트가 입력한 데이터를 어떤 식으로 전송할지(GET or POST)

```html
<form action="exmaple.php" method="post">
</form>
```
=> 위의 예제는 example.php 라는 서버 프로그램으로 입력값을 전송하여 요청할 것이다. POST 방식으로 전송할 것이다.

### GET vs POST
GET: 서버에 요청을 보내어 응답을 받아낸다. 서버로부터 정보를 '가져오겠다'는 성격의 요청이다.   
POST: 서버에 요청을 보내어 작업을 수행한다. 서버에 있는 데이터를 추가/수정/삭제 한 후에 응답을 받아낸다.   
서버의 정보를 '조작하겠다'는 성격의 요청이다.

### 실전
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>서버에 요청을 보내자, 폼!</title>
    </head>
    <body>
        <h1>키우고 싶은 동물 고르기</h1>
        <form action="exam.php" method="POST">
            <input type="text" placeholder="NAME" name="name">
            <br>
            <select name="pet">
                <option value="dog">강아지</option>
                <option value="cat">고양이</option>
                <option value="parrot">앵무새</option>
            </select>
            <br>
            <input type="submit" value="전송">
        </form>
    </body>
</html>

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>서버에 요청을 보내자, 폼!</title>
    </head>
    <body>
        <h1>키우고 싶은 동물 고르기</h1>
        <form action="exam.php" method="POST">
            <input type="text" placeholder="NAME" name="name">
            <br>
            <select name="pet">
                <option value="dog">강아지</option>
                <option value="cat">고양이</option>
                <option value="parrot">앵무새</option>
            </select>
            <br>
            <input type="submit" value="전송">
        </form>
    </body>
</html>