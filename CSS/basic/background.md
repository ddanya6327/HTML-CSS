# Background

## background-color

- 배경의 색상을 지정할 수 있다.
  - hex
  - rgb
  - rgba

## background-image

- 배경 이미지를 넣을 수 있다.
  - url 함수를 사용해야 함.

```css
.box {
  background-image: url("./image.jpg");
}
```

## background-repeat

- 배경 이미지의 반복값을 설정
  - repeat
  - no-repeat

## background-size

- contain
  - 요소 안에 이미지 전체가 나오도록 설정
- cover
  - 요소 안에 빈 공간이 남지 않도록 꽉 참 (이미지는 잘릴 수 있음)
- custom

## background-position

- 이미지를 어디에 위치 시킬지
  - x
  - y
  - center

```css
.box {
  background-image: url("./image.jpg");
  background-position: left top;
  /* background-position: 25px 15px; */
  /* background-position: center center; */
  /* background-position: 50% 30%; */
}
```
