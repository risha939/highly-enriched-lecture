# Tag

### 빠른 시작
! + enter


### 문자를 꾸며주는 태그

```html
// html                        // Browser에 그려짐
<strong>Hello World</strong>   <!-- **Hello World(두꺼움)** -->

<u>Hello World</u>             <!-- Hello World(밑줄) -->

<h1>Hello World</h1>           <!-- 큰사이즈의 제목. **h1부터 h6까지 (점점 작아짐)**-->

```

### 빈 태그

```html
<br />     // 다음 줄로 내려가는 태그
<hr />     // 수평선을 그려주는 태그
```

### 특정 기능이 있는 태그와 속성 (attribute, value)

❗️ 속성과 값은 중첩이 가능합니다. ❗️

```html
// 기능이 있는 태그*

<button>버튼</button>                <!-- 버튼 생성 -->
<textarea>입력창</textarea>          <!-- 여러줄 텍스트 입력창 생성 -->

// 태그의 attribute와 value

<input type="text" />               <!-- 한줄 텍스트 입력창 생성 -->
<input type="password" />           <!-- 비밀번호 입력창 생성 -->
<input type="color" />              <!-- 색상 선택창 생성 -->
<input type="checkbox" />           <!-- 체크박스(여러개선택) 생성 -->
<input type="radio" name="group"/>  <!-- 라디오버튼(1개선택) 생성 -->
    => name이 동일한 radio 버튼 중 1개만 선택됨

<label>라벨</label>  <!-- 체크박스, 라디오버튼 등에 라벨 생성 -->

<a href="<http://google.com>">구글로 가기</a>                 <!-- 현재창에서 이동-->
<a href="<http://google.com>" target="_blank">구글로 가기</a> <!-- 새창에서 이동 -->
```

### 이미지와 동영상 태그

```html
<!-- 일반이미지 -->
<img src="/이미지경로/이미지.확장자" />

<!-- 배경이미지 -->
<div style="background-image: url('/이미지경로/이미지.확장자')" />

<!-- 동영상 -->
<video muted="muted" autoplay="autoplay" loop="loop">
	<source src="동영상위치.mp4">                    <!-- muted: 음소거 -->
</video>                                          <!-- autoplay: 자동재생 -->
                                                  <!-- loop: 반복재생 -->
```

### Block, Inline

```html
<!-- Block 요소 -->
<h1 />
<div />
<p />

<!-- Inline 요소 -->
<span />
<input />     <!-- text, checkbox, radio 모두 동일 -->
<a />
<button />
<label />
```

# HTML 문서구조 및 설명

```html
// HTML5 버전 선언 방법
<!DOCTYPE html>
<html>
	// 검색엔진을 위한 영역
	<head>
		<title>사이트 이름</title>
		<meta name="description : 사이트 소개" content="사이트 소개"/> 
		<meta property="og:image" content="image.png"/>          <!-- 다른 사이트(카톡 등)에 이미지 알리기 -->
		<meta property="og:title" content="title"/>              <!-- 다른 사이트(카톡 등)에 사이트명 알리기 -->
		<meta property="og:description" content="description"/>  <!-- 다른 사이트(카톡 등)에 사이트상세 알리기 -->
	</head>

	// 브라우저에서 보여지는 영역
	<body>
		<header></header>           <!-- 웹페이지의 상단(또는 상단메뉴) 부분 -->
		<nav></nav>                 <!-- 웹페이지의 좌측(또는 우측메뉴) 부분 -->
		<section></section>         <!-- 웹페이지의 독립적인 섹션 부분 -->
		<article></article>         <!-- 웹페이지의 블로그, 뉴스, 기사 등 -->
		<footer></footer>           <!-- 웹페이지의 하단 기업정보 부분 -->
	</body>
</html>
```