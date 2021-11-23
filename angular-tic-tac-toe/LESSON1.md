# Angular

npm을 패키지 관리자로 사용하는 Progressive web app이다.

javascript + css + html언어를 사용하고 nodejs기반의 webpack을 사용하는 기술이다.

## Webpack 특징

기본은 여러개의 자바스크립트 파일을 하나의 bundle.js로 묶어주는 기술이다.

이렇게 하면 여러가지 장점이 있다.

1. 용량이 줄어들어 전송에 용이해짐
2. 모듈 단위 개발이 가능
3. 라이브러리 순서를 고려할 필요가 없음.
4. ES6 이상의 스크립트 사용 가능. (기존 ES5 버전으로 변경해줌)

## Angular 특징

Angular 프레임워크는 핫 리로드를 지원하는 점이 가장 핵심.

webpack으로 번들링된 앱은 코드 변경할 때마다 빌드되어 변경점이 화면에 표출된다.

Angular2부터 타입스크립트를 쓰며 웹 프레임워크 중 가장 먼저 도입했다.

- 코드 변환 과정 요약: 
    - typescript -> javascript(ES6, ES5) -> bundle.js(ES5)



테스팅 프레임워크는 jasmine, jest, sybres 등이 있다. 

## Angular 시작하기

우선 Angular cli가 있어야 한다.
```
npm install -g @angular/cli
```
cli 실행 이후 다음의 간단한 커맨드로 기본 앱 생성이 가능하다.
```
ng new my app
```

## 기본 구성

### 1. Component
- selector : html에서 쓸 명칭
- template : 각 컴포넌트에서 담을 html. 별도의 html 파일로 존재하기도 한다.

    - 부모 객체에서 자식객체로 데이터를 넘길 경우 [X] = "" 형태로 넘기고 @input() X: 을 통해서 전달받는다.
- style : css 스타일
- class : data 처리 로직을 담음
### 2. html
- html 코드들을 담고있으며 component를 배치 할 수 있음.
- 컴포넌트 내부 데이터를 {{ Y }} 형태로 표출 가능하다.
- ngif를 통해서 html 내부에서 if 분기 가능.
- ngfor를 통해서 html 내부에서 for문 처리 가능.


### 3. css
### 4. spec (optional testing file)
- jasmin 문법을 통해서 테스트 구성 가능

