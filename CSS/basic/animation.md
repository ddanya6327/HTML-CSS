# Animation

```css
.box {
  position: relative;
  animation-name: move-box;
  animation-duration: 2000ms;
}

@keyframes name {
  from {
    top: 0;
  }

  to {
    top: 200px;
  }
}
```

```css
@keyframes name {
  0% {
  }

  50% {
  }

  100% {
  }
}
```

## animation-duration

- 재생 시간
  - ms
  - s

## animation-timing-function

- 재생속도
  - ease-in
  - ease-out
  - ease-in-out
  - cubic-bezier()

## animation-delay

- 딜레이
  - ms
  - s

## animation-iteration-count

- 반복 횟수
  - 정수를 입력하거나 infinite 를 입력 할 수 있음

## animation-direction

- 애니메이션 진행 방향
