## Table

```html
<table>
  <thead>
    <tr>
      <th>table header</th>
      <th>table header2</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>table data</td>
      <td>table data2</td>
    </tr>
    <tr>
      <td rowspan="2">table data</td>
    </tr>
    <tr>
      <td colspan="3">table</td>
    </tr>
  </tbody>

  <tfoot></tfoot>
</table>
```

# Media

- image, audio, video 같은 파일을 첨부 할 때 사용.

## Audio

```html
<audio src="./audios/test.mp3" controls></audio>

<audio controls>
  <source src="./audios/test.mp3" type="audio/mp3" />
  <source src="./audios/test.wav" type="audio/wav" />
  <p>음악을 재생할 수 없습니다.</p>
</audio>
```

### Attributes

- src
  - 경로
- controls
  - audio의 컨트롤 패널을 표시한다.
- autoplay
  - 자동 재생
- loop
  - 반복 재생

## Video

```html
<video src="./videos/test.mov" controls></video>

<video controls>
  <source src="./audios/test.mov" type="video/mp4" />
  <source src="./audios/test.mp4" type="video/mp4" />
  <p>영상을 재생할 수 없습니다.</p>
</video>
```

### Attributes

- src
  - 경로
- controls
  - audio의 컨트롤 패널을 표시한다.
- autoplay
  - 자동 재생
- loop
  - 반복 재생

## Iframe

- HTML 안에 또 다른 HTML을 사용하고 싶을 때
  - 유튜브의 영상 같은거 공유 할 때 주로 사용?

```html
<iframe src="https://www.youtube.com"></iframe>
```

---

## Abbreviation

- 약어의 원형을 표현 할 수 있는 태그

```html
<p>
  너 혹시 <addr title="Attention Deficit Hyperactivity Disorder">ADHD</addr>니?
</p>
```

## Address

- 연락처에 대한 내용을 마크업 할 수 있다.

```html
<address>
  <h1>
    youtube yang
  </h1>
  <a href="https://www.youtube.com">youtube</a>
</address>
```

## Preformatted

- 공백 등 입력한 형식 그대로 출력하는 태그

```html
<pre>
  내가 입력한
  대로 출력이
  됩니다.
</pre>
```

## Code

- Code를 입력할 때 사용한다.
  - indent 를 표현하기 위해 pre와도 같이 사용 함.

```html
<pre>
    <code>
        console.log('hello world');
    </code>
</pre>
```
