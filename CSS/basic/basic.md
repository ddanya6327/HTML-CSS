# CSS

## CSS의 기본 구조

```css
selector {
  property: value;
}
```

## Style의 작성 방법 3가지

- .css 파일을 link를 통해 불러오기

  - 가장 권장되는 방법

- HTML의 header 안에 style 태그를 통해 작성

- 태그의 style attribute를 사용해서 작성
  - 일반적으로 사용하지 않는 편이 좋다. 유지보수가 어려움

## CSS의 우선 순위

- 기본적으로 같은 선택자에 여러 스타일이 선언 된 경우, 마지막에 선언된 스타일을 적용한다.

```css
p {
  color: blue;
}

p {
  color: red;
}

/* 위의 경우 마지막에 선언한 color:red; 가 적용된다. */
```

- 단, 우선순위가 적용된다.

  - ID > Class, Pseudo-class > Type

```html
<p id="text" class="a b c d e"></p>
```

```css
#text {
  color: blue;
}

.a .b .c .d .e {
  color: red;
}

/* 위 경우, .a .b 같은 class의 스타일을 적용하는 코드를 마지막에 작성했지만,
   ID의 우선권이 더 높기 때문에 p태그의 color는 blue가 된다. */
```

```css
.box p {
  color: blue;
}

p {
  color: hotpink;
}

/* 위의 경우에도 class의 우선순위가 type보다 높기 때문에 p의 컬러는 blue가 된다. */
```

```css
li:last-child {
  /* last-child는 가상 클래스 이므로 class와 우선 순위가 동일하다. */
  /* li는 type */
}
```

- inline-style 의 경우 어떤 스타일보다 우선 순위가 높다.

  - inline-style > ID > class > type

## !important

- 가장 우선권이 높다. (inline-style 보다 높음)

  - 누군가가 이걸 사용해두면 어떤 것을 해도 CSS가 적용 되지 않는 경우가 있다.

```css
p {
  color: red !important;
  /* 우선 순위가 가장 높으므로 최우선 */
}
```
