# Box-model

모든 HTML 요소는 박스(BOX) 모양으로 구성되며, 이것을 박스 모델이라 부른다.

- Content

  - 가로는 width, 세로는 height로 표기

- Padding

  - 안쪽 여백, content와 border 사이의 공간

- Border

  - 테두리
  - 굵기, 스타일, 색상을 지정 해줘야 한다.

- Margin
  - 바깥 여백, 요소와 요소의 간격을 나타낼 때 사용

## 속기형 (Shorthand)

```css
.box {
  margin: 10px 20px 30px 40px;
}
```

- top right bottom left 의 순서로 값을 지정할 수 있다.
  - top: 10px, right: 20px, bottom: 30px, left: 40px; 라고 선언 한 것

# Box-sizing

Box의 Size를 어떤 것을 기준으로 계산할지 정하는 속성

1. content-box : 콘텐트 영역을 기준으로 크기를 정합니다.
2. border-box : 테두리를 기준으로 크기를 정합니다.
3. initial : 기본값으로 설정합니다.
4. inherit : 부모 요소의 속성값을 상속받습니다.

- 기본 값은 content-box인데 이 속성은 content box의 값만을 기준으로 한다. 그래서 padding 의 값을 추가해도 content box의 값은 동일하고 padding의 값이 추가 됨.

- 예를 들어, box-sizing: border-box; 로 하면 border 까지 포함한 width, height를 계산해서 content 의 크기를 지정해준다.
  - content의 width가 400인 경우, padding에 40px 속성을 준다면, content + padding = 440이 되지만, box-sizing이 border-box인 경우, padding의 40값을 자동으로 계산하여 width가 400이 되도록 content의 값을 자동으로 360으로 설정한다.

```css
* {
  box-sizing: border-box;
}
/* 모든 요소들의 box-sizing을 border-box를 기준으로 한다. */
```
