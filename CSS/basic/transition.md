# Transition

- 변화가 필요 할 때, 애니메이션을 통해 변화 할 수 있도록 하는 속성

transition: property duration \[timing-function\] \[delay\]

```css
.box {
  transition: font-size 2500ms;
}

/* 개별적으로도 선언 가능하다 */
.box {
  transition: font-size 1000ms ease-out, background-color 2000ms cubic-bezier(
        0.08,
        0.57,
        0.97,
        -0.78
      ) 1000ms;
}
```

## property

- 어떤 항목에 적용할지

## duration

- 애니메이션 시간
  - ms
  - s

## timing-function

- 재생 속도 조절
  - ease-in
  - ease-out
  - ease-in-out
  - cubic-bezier()

## delay

- 재생시 딜레이
