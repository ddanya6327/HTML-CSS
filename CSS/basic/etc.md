# Box-shadow

- 박스 그림자

- box-shadow: h-offset v-offset blur spread color

```css
.box {
  box-shadow: 0 10px 16px 0 rgba(255, 73, 73, 0.35);
}
```

- 4개만 적으면 spread 생략
- 3개만 적으면 blur spread 생략

# Opacity

- 불투명도

```css
.box {
  opacity: 0.1;
}
```

# Overflow

- 종류

  - overflow-x
  - overflow-y

- 속성
  - visible
  - auto, scroll
  - hidden

# Transform

- Transform의 대표적인 함수
  - translate(x,y)
    - 자기 자신을 이동시킬 때
  - scale(N)
    - 자기 자신의 사이즈를 N 만큼 변경함
  - sclae(x,y)
    - x축은 x만큼, y축은 y만큼 사이즈를 변경함
  - rotate(Ndeg)
    - 자기 자신을 N 만큼 회전시킴

```css
.box {
  transform: rotate(45deg);
}
```

- transform 함수로 변형시킬 경우 주변 요소에 영향을 주지 않음.

# Visibility

- 해당 요소를 표시 할지, 표시 안할지

  - visible
  - hidden

- 해당 요소를 표시하지 않더라도 영역은 가지고 있다.
  - display none의 경우는 없는 존재로 취급해서 공간이 비어버리거나 하지만, visibilty: hidden의 경우 공간을 차지함.
