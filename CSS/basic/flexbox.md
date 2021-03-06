# Flexbox

- https://developer.mozilla.org/ko/docs/Learn/CSS/CSS_layout/Flexbox

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

## Flex-grow

- 컨테이너가 커질 때 어떤 비중으로 커질지
  - 0 또는 양의 정수를 사용하는데, 0을 설정 해주면 container의 크기가 커져도 원래 크기를 유지함.

```css
.item {
  flex-grow: 1;
}
```

## Flex-shrink

- 컨테이너가 작아 질 때 어떤 비중으로 작아질지
  - 0 또는 양의 정수를 사용하는데, 0의 경우 container가 작아져도 item의 크기가 줄어들지 않음.

```css
.item {
  flex-shrink: 1;
}
```

## Flex-basis

- container의 크기에 따른 item 의 크기 기준을 나눌 수 있음.
  - px, em, rem, % 단위를 사용 할 수 있음.
  - 기본 값은 auto

```css
.item1 {
  flex-basis: 60%;
}

.item2 {
  flex-basis: 40%;
}
```

## Align-self

- 한 아이템에 대한 align 속성

```css
.item1 {
  align-self: center;
  /* item1 요소만 중간 정렬 */
}
```

## 자주 사용하는 FlexBox 속성 10가지

- https://d2.naver.com/helloworld/8540176
