## Form

- 사용자로부터 인풋(Input)을 받기 위한 Tag

```html
<form action="URL" method="GET"></form>
```

### Attributes

- action
  - form의 내용을 전송할 URL 주소
- method
  - GET | POST

## Input

```html
<input type="text" placeholder="default" minlength="5" maxlength="13" />
<input type="text" value="name" />
<input type="text" required />
<input type="text" desabled />
```

### Attributes

#### 필수

- type
  - text
  - email
  - password
  - url
  - number
    - max, min 속성을 사용해서 최대값, 최소값을 할 수 있다.
  - file
    - accept 속성을 사용해서, 허용하고자 하는 파일 형식을 정할 수 있다.
    - ex) accept=".png, .jpg"

#### 선택

- placeholder
  - 기본 값
- maxlength
  - 글자 제한(최대값)
- minlength
  - 글자 제한(최소값)
- required
  - 필수 항목
- desabled
  - 사용 불가
- value
  - 값

## Label

- 폼 양식에 이름을 붙이는 태그

```html
<label for="user-name">name</label> <input type="text" id="user-name" />
```

### Attributes

- for
  - input과 연결하기 위한 값. input의 id를 입력한다.
