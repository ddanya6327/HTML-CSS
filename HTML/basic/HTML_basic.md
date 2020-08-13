# !DOCTYPE html

- 이 문서가 HTML5 버전임을 알리기 위한 태그
  - 문서의 최상단에 선언

```html
<!DOCTYPE html>
<html>
  <head>
    ...
  </head>

  <body>
    ...
  </body>
</html>
```

# HEAD

## Title

- HTML 문서의 제목

```html
<head>
  <title>Title test</title>
</head>
```

- 각 페이지 마다 그에 맞는 타이틀을 써주는데 검색 최적화(SEO)에 좋음

## Link

- 다른 파일을 불러올 때 사용.
  - CSS, Font 등

```html
<head>
  <link rel="stylesheet" href="./styles.css" />
</head>
```

## Style

- HTML 문서 내에 CSS를 작성할 때 사용한다.

```html
<head>
  <style>
    h1 {
      color: red;
    }
  </style>
</head>
```

## Script

- HTML 문서 내에 JavaScript 파일을 첨부 할 때 사용
  - head에 명시하면 body의 요소를 사용하지 못하므로 body의 가장 마지막에 작성하거나 defer를 사용하자.

```html
<body>
  <script src="./app.js"></script>

  <script>
    console.log("hello world");
  </script>
</body>
```

## Meta

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

### Attributes

- name
  - 메타 데이터의 종류
    - 자주 쓰는 메타 데이터 (MDN 사이트 참조)
      - viewport
      - author
      - keywords
      - description
- content
  - 메타 데이터 값
