### 특성 (property)

```css
div {
    color: red;
    color: rgb(255,0,0);      /* RGB */
    color: #FF0000;           /* HEX 값 */

    font-size: 20px;          /* 글자크기 */
    font-weight: 300;         /* 글자두께 */
    text-align: center;       /* 가운데 정렬 */
    font-family: arial;       /* 글꼴 */

    width: 300px;             /* 넓이 */
    height: 300px;            /* 높이 */
    background-color: red;    /* 배경색 */
    border: 1px solid black;  /* 테두리 */
    border-radius: 5px;       /* 테두리의 모서리 둥글게 */
}
```

### 기본문법

#### 단일 속성
```css
selector(선택자) {
    property(속성) : value(값) ;
}
```

#### 다중속성
```css
selector(선택자) {
    property(속성) : value(값) ;
    property(속성) : value(값) ;
    property(속성) : value(값) ;
    property(속성) : value(값) ;
    property(속성) : value(값) ;
}
```

# CSS 사용방법

### html 태그에 입력

- html 태그에 직접 입력하는 것은 코드가 뒤섞여 유지보수 측면에서 매우 비효율적
- html 파일 사이즈를 크게 만들어 로딩 시간이 늘어남

### style 태그에 입력

- 코드가 뒤섞여 있진 않으나, < head > 태그가 로드되는 하위의 모든 html 페이지에 css가 적용됨 (분리적용 불가)

### css 파일 분리

- 위의 단점들을 해소할 방법임 실무에서 가장 많이 사용되는 중

```html
// 별도의 css 파일을 html 파일에 적용시키는 법
<head>
    <link href="style.css" rel="stylesheet" />
</head>
```

# 선택자

```css
<!-- CSS 기본 선택자 -->
<style>
    * { color: red; }                      // 전체 선택자

    tag { color: red; }                    // 태그 선택자

    .class { color: red; }                 // 클래스 선택자

    #id { color: red; }                    // 아이디 선택자

    선택자:가상상황 { background-color: red; } // 가상 선택자
</style>
```

❗️ 선택자는 tag ⇒ class ⇒ id 순으로 우선순위 적용 ❗️