# Flexbox

## 선언

- 정렬 하고자 하는 요소를 지닌 부모의 display에 flex 또는 inline-flex를 선언한다.

```css
.flexbox {
  display: flex;
  /* flex | inline-flex */
}
```

- 어느 방향으로 정렬을 할 것인지?
  - flex-direction 속성을 통해 정의

```css
.flexbox {
  display: flex;
  flex-direction: row;
  /* row | row-reverse | column | column-reverse */
}
```

- 모든 요소를 한 줄에 정렬 할 것인지, 여러줄로 할 것인지
  - flex-wrap 속성으로 정의
  - nowrap 의 경우 자식의 사이즈를 줄여서라도 한줄을 유지한다.
  - wrap 의 경우 여러줄이 되더라도 자식의 크기는 줄이지 않음

```css
.flexbox {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  /* wrap | nowrap */
}
```

## main-axis, cross-axis

- justify-content

  - main-axis를 기준으로 요소를 정렬

- align-items, align-content
  - cross-axis 를 기준으로 요소를 정렬

## order

- 자식 요소에 order 속성을 줘서 순서를 정할 수 있다.

```css
.red {
  order: 1;
}

.yellow {
  order: 2;
}
```
