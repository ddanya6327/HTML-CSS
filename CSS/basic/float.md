# Float

요소를 가로 배치 하기 위해 사용.

특징

1. float 속성을 갖는 요소는 html 문서에서 공간은 차지하지만, 다른 요소의 배치에 영향을 안주게 된다. (빈 자리로 인식)

- 즉 요소의 위치가 겹칠 수 있으며, 자식 요소에 따라 height가 결정되는 부모 box의 경우, float 요소의 height는 포함하지 않게 된다. (float 속성 끼리는 충돌)

- 자식 요소 모두가 float 속성을 가지고 있다면, 부모의 height가 0이 될 수 있다.

2. float 속성을 추가하면 block 속성이 된다.

- inline 같은 속성을 가진 요소의 display를 float로 설정하면 inline -> block 형태로 바뀐다.

3. display 속성이 block이 되면, 남은 공간을 margin으로 채우거나 하는 특징이 있지만, 이 경우는 따로 margin을 생성하거나 하지 않음. (margin을 줄 수 없다는건 아니고 자동으로 생기는 margin이 생기지 않는다는 뜻.)

- 그래야 가로로 여러가지 요소를 배치 할 수 있기 때문?

4. inline의 요소들은 float 된 요소들과 충돌한다.

---

float tips

- float 요소를 가진 부모에게 overflow: hidden 속성을 주면 float 된 자식의 height 값을 알 수 있게 된다.

  - height 100px 크기의 box가 float 속성을 가지고 있다면, 부모의 height는 0px가 되지만, 부모에게 overflow: hidden 옵션을 주게 되면 float 속성을 가진 요소를 인식하게 됨.
  - 정확한 원리를 모르기 때문에 사용하지 않는 편이 좋을 것 같다.

- clear: left

  - 이 속성을 주면 float가 아닌 요소들이 float: left 로 된 요소를 인식할 수 있게 된다.
  - a요소가 float 속성을 가지고 있고 b요소에 float: left 속성을 주면 b가 a를 인식 할 수 있게 되어서 겹치지 않게 된다.
  - clear는 left, right, both 속성이 있음.

- float 로 가로 정렬을 할 경우, clear: left 속성을 가진 div 라던지를 마지막에 주지 않으면 이상하게 출력 될 확률이 있다. 근데 그렇다고 의미 없는 div를 넣기는 그러니까 css의 가상 요소를 넣어서 처리하면 좋다.
  - 가상 요소에서 content는 필수
  - display도 block으로 해주자

```css
.div::after {
  content: "";
  display: block;
  clear: left;
}
```
