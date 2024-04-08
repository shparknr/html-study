# 2. 스타일

## 2.1. 스타일 시트

- 브라우저 기본 스타일
  - 웹 브라우저에서 기본으로 사용하는 스타일
- 인라인 스타일
  - style 속성을 사용해서 필요한 요소에 스타일 직접 지정
- 내부 스타일 시트
  - 문서 앞부분(head 안)에 스타일을 모아서 함께 정리하고 관리
- 외부 스타일 시트
  - 스타일을 따로 파일로 저정한 후 연결

## 2.2. css 기본 선택자 (selector)

1. 전체 선택자

- 문서 모든 요소에 스타일을 적용

```css
* {
  margin: auto;
}
```

2. 타입 선택자

- 특정 태그를 사용한 모든 요소에서 스타일을 적용

```css
p {
  font-style: italic;
}
```

3. 클레스 선택

- 특정 부분만 선택해서 문서 안에 여러번 적용

```css
.form-wrap {
  background-color: #ddd;
}
```

4. 그룹 선택자

- 여러 요소에 같은 스타일을 적용

```css
h1,
h2,
ul,
li {
  text-align: center;
}
```

5. id 선택자

```css
- #id {
  color: #fff;
}
```

## 2.3. 스타일 우선순위

1. 얼마나 중요한가?

- 사용자 스타일 -> 제작자 스타일 -> 브라우저 기본스타일

2. 적용 범위 어디까지인가?

- !important -> 인라인 스타일 -> id 스타일 -> 클래스 스타일 -> 타입 스타일

3. 소스 작성 순서

- 나중에 작성한 스타일이 먼저 작성한 스타일을 덮어쓴다.

## 3. 텍스트 스타일

## 3.1. 글자와 관련된 속성

- font-family: 글꼴 종류 지정
- font-size: 글자 크기 지정
- font-style: 글자 이탤릭체로 표시할지 지정
- font-weight: 글자 굵기 지정

## 3.2. 택스트 스타일 속성

- color: 글자 색 지정
- text-decoration: 택스트에 밑줄, 취소선 표시할지 여부
- text-transform: 택스트 전체, 또는 첫 글자를 대문자로 표시할지 여부
- text-shadow: 택스트에 그림자 추가
- letter-spacing: 글자 사이의 간격 (자간)
- word-spacing: 단어 사이의 간격
- text-align: 택스트 정렬 방법 지정
- line-height: 줄 간격 조절 (행간)

## 3.3. 웹에서 색상을 지정하는 방법

- 16진수 Hex: #000
- rgb, rgba: rgba(255, 255, 255, 0.7(투명도))
- hsl, hsla
- 색상이름, white, black

## 3.4. 텍스트를 정렬하는 text-align

- start: 현재 텍스트 줄의 시작 위치에 맞추어 문단을 정렬
- end: 현재 텍스트 줄의 끝 위치에 맞추어 문단을 정렬
- left: 왼쪽 맞춤
- right: 오른쪽 맞춤
- center: 가운데 맞춤
- justify: 양쪽 맞춤
- match-parent: 부모 요소를 따라 문단 정렬

## 3.5. 줄 간격을 조절하는 line-height

- 보통 1.25 ~ 1.75배 정도 추천

## 3.6. 텍스트의 줄을 표시하거나 없애주는 text-decoration 속성

- 텍스트의 밑줄을 긋거나 취소선을 표시
- 하이퍼링크 밑줄 없애기 등에 사용
- none
- underline
- overline
- line through

## 3.7. 텍스트에 그림자 효과 text-shadow 속성

- text-shadow: 가로거리 세로거리 번짐정도 색상

## 3.8. 텍스트의 대소문자를 변환하는 text-transform 속성

- 영문자
- capitalize: 첫 번째 글자를 대문자로
- uppercase: 모든 글자를 대문자
- lowercase: 모든 글자를 소문자
- full-width: 가능한 모든 문자를 전각(가로세로폭이 동일한) 문자로 변환

## 3.9. 글자 간격을 조절하는 letter-spacing, word-spacing

- letter-spacing: 자간
- word-spacing: 단어와 단어사이의 간격을 조절
