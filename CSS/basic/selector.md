# Selector

## Type Selector

- HTML 태그를 지칭

```css
h1 {
  color: blue;
}

strong {
  color: yellow;
}
```

## Class Selector

- Class 요소를 선택

  - .box = box라는 클래스를 선택

```css
.box-0 {
}

.box-0.box-1 {
  /* 이런 형태로도 사용 할 수 있다. */
}
```

## ID Selector

- ID 요소를 선택

```css
#yang {
  ...;
}

.box#yang {
  /* class가 box면서 id가 yang인 태그 */
}
```

---

## Child Combinator

```HTML
<section>
    <h1>TEST</h1>
    <ol>
        <li>1</li>
        <li class="active">2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
    </ol>
</section>
```

- 자식 선택자
  - parent > child

```css
section > h1 {
  /* section의 h1이 선택 됨 */
}
```

## Descendants Combinator

- 자손 선택자
  - parent child

```css
section li {
  /* section의 자손인 li가 선택됨 */
}
```

## Sibling Combinators

- 형제 선택자

  - parent + sibling
    -
  - parent ~ sibling

```css
.active ~ li {
  /* active 클래스의 형제 요소중 모든 li를 선택 */
}

.active + li {
  /* active 클래스의 형제 요소중 첫번째 li를 선택 */
}
```

---

# Pseudo-classes

```HTML
<section>
    <h1>TEST</h1>
    <ol>
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
        <li>6</li>
    </ol>
</section>
```

## Structural Pseudo-classes

- 구조적 가상 클래스 선택자

  - element:first-child

  - element:last-child

  - element:nth-child(n)

- 가상 클래스를 사용하면 `<li class="first-child">` 와 같은걸 사용할 필요가 없어진다.

```css
li:first-child {
  /* li의 첫번째 요소 */
}

li:last-child {
  /* li의 마지막 요소 */
}

li:nth-child(3) {
  /* li의 세번째 요소 */
}

li:nth-child(2n) {
  /* li 의 짝수 요소 */
}

li:nth-child(2n-1) {
  /* li의 홀수 요소 */
}
```

## User Action Pseudo-classes

- 동적 가상 클래스 선택자
  - 어떤 상태나 조건에 따라 달라질 수 있는 경우 사용

```css
a:hover {
  /* a태그에 마우스를 올렸을 때 */
}

a:active {
  /* a태그를 눌렀을 떄 */
}

input:focus {
  /* input에 focus가 되었을 때 */
}
```
