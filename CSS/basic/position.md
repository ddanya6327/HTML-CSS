# Position

## static

- 모든 요소의 기본 포지션 값

## relative

- 자기 자신이 있던 자리를 기준으로 이동

## absolute

- 부모 요소 중 position이 static 아닌 요소를 기준으로 위치를 정함

- display 속성이 block 으로 바뀜
  - float와 같이 다른 요소와 충돌하지 않는 block

## fixed

- viewport 를 기준으로 위치를 정함

- absolute 처럼 속성이 block으로 바뀜

## sticky

---

## 포지션을 옮기는 속성

- 위치

  - top
  - left
  - right
  - bottom

- z-index

  - 수직 방향의 위치를 정하기 위해 사용.

- modal 같은거 정 가운대 배치 하는 방법
  - left: 50%;
  - transform: translate(-50%, -50%);
