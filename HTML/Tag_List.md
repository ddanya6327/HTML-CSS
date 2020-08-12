## Title

```html
<h1>Title</h1>
<h2>Title2</h2>
...
<h6>Title6</h6>

<p>p</p>
```

## Emphasis

```html
<em> Emphasis </em>
<string> Emphasis </strong>
```

## Anchor

```html
<a href="address" target="_blank">link</a>
```

### Attributes

- href
  1. web URL
  2. page
  3. e-mail (mailto:address)
  4. tel (tel:012345678)
- target="\_blank"
  - 새로운 탭을 열어서 이동

## Image

```html
<img src="https://bit.ly/2mvVsGI" alt="cat" />
```

Attributes

- src (source)
- alt (alternative text)

## List

```html
<ul>
  <li>hi</li>
  <li>hi2</li>
</ul>
```

- ol (ordered list)
  - 순서가 중요한 목록
- ul (unordered list)
  - 순서가 중요하지 않은 리스트
- li (list item)
  - 항목

> ul과 ol의 자식 요소는 무조건 li만 사용할 수 있다.

## Description List

```html
<dl>
  <dt>
    <dfn>development</dfn>
  </dt>
  <dd>1. 발달 , 성장</dd>
  <dd>2. 개발, 신개발품</dd>
</dl>
```

무언가를 정의 할 때 사용하는 태그

- dl (description list)
- dt (description term)
- dd (description data)
- dfn

> dl의 자식 요소는 오직 div, dt, dd만 가능하다.

## Quotations

- 인용문에 사용 한다.

### Blockquote

- 문단을 인용할 때 사용한다.

```html
<blockquote cite="https://google.com">
  <p>block quote test</p>
</blockquote>
```

- 출저가 URL인 경우
  - blockquote의 속성에 표기

```html
<blockquote cite="https://google.com">
  <p>block quote test</p>
</blockquote>
```

- 출저가 텍스트인 경우
  - cite 태그를 사용

```html
<blockquote>
  <p>block quote test</p>
  <cite>Albert Einstein</cite>
</blockquote>
```

### Q tag

- 특정 부분을 인용할 때

```html
<q>Quotations test<q></q></q>
```

## Div

- 요소를 묶을 때 사용한다.

```html
<div>
  <h1>div test</h1>
</div>
```

## Span

- 요소를 묶을 때 사용한다. (text level)

```html
<span>span test</span>
```
