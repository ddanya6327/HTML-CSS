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

## Radio

- 여러 항목 중 하나를 선택할 수 있다. (name 속성이 같은 값 끼리)

```html
<form>
  <input type="radio" name="subscription" value="subscribed" id="subscribed" />
  <label for="subscribed">subscribed</label>
  <input
    type="radio"
    name="subscription"
    value="unsubscribed"
    id="unsubscribed"
  />
  <label for="unsubscribed">unsubscribed</label>
</form>
```

## Checkbox

- 여러 항목을 체크 할 수 있다. (name 이 같은 속성 끼리)

```html
<form>
  <input type="checkbox" name="skills" id="html" />
  <label for="html">HTML</label>
  <input type="checkbox" name="skills" id="css" />
  <label for="html">CSS</label>
  <input type="checkbox" name="skills" id="js" />
  <label for="html">JavaScript</label>
</form>
```

## Select

- 항목을 선택 할 수 있다.

```html
<form>
  <label for="skill">Skill</label>
  <select multiple name="skill" id="skill">
    <option value="html">HTML</option>
    <option value="css">CSS</option>
    <option value="js">JavsScript</option>
  </select>
</form>
```

### Attributes

- multiple
  - 여러 항목을 선택할 수 있다.

## Textarea

```html
<label for="field">자기소개:</label>
<textarea id="field" placeholder="자기소개를 입력하세요"></textarea>
```

### Attributes

- rows
  - 행 길이
- cols
  - 열 길이

## Button

```html
<button type="button">
  button
</button>
```

### Attributes

- type
  - button
    - 기본적인 button
  - submit
    - form 을 전송할 때
  - reset
    - form 을 리셋할 때
