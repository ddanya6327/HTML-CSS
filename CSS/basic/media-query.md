# Media Query

- PWA 를 만들기 위해 사용
- 반응형 웹을 정상적으로 사용 하려면, meta태그에 viewport 를 명시 해야 한다.

```html
<meta name="viewport" content="width=device-width" />
```

## Media Query 선언

- @media 를 통해 선언 (@media screen and)

```css
@media screen and (min-width: 576px) {
  /* css */
}

@media screen and (min-width: 768px) and (max-width: 991px) {
  /* css */
}
```
