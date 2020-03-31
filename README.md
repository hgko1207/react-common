# React

## React 기능

- Component
- Context
  - createContext
- Hooks
  - useState
  - useRef : 일반 값을 기억
  - useEffect : componentDidMount, componentDidUpdate, componentWillUnmount
  - useLayoutEffect
  - useMemo : 복잡한 함수 결과 값을 기억(함수의 리턴 값을 기억)
  - useCallback : 함수 자체를 기억, 자식 컴포넌트에 함수를 전달 시 무조건 사용, 이벤트 함수에 거의 사용
  - useReducer : reducer를 편리하게 사용하기 위해
  - useMemo : 함수형 컴포넌트 내부에서 발생하는 연산을 최적화 할 수 있음.
  - useContext : context 사용하기 위해
- PureComponent : Class Component 일 때 사용
- memo : Function 일 때 사용
- React Router

## React 설치

```bash
// Install
npm i or yarn add

// Basic
yarn add react react-dom
yarn add prop-types

// React Router
yarn add react-router
yarn add react-router-dom

// Rest api
yarn add axios

// Style
yarn add styled-components
yarn add styled-reset
yarn add styled-flex-component
yarn add react-bootstrap bootstrap
yarn add typography

// Compoentns
yarn add react-textarea-autosize
yarn add copy-to-clipboard
yarn add react-helmet
yarn add react-tabs

// Icons
yarn add react-fontawesome
```

## React Router

- Link
- Route
  - render props : 자식에게 부모 props를 전달하고 싶을 경우
  - exact : path와 정확하게 일치하는 경우
- Browser
  - BrowserRouter
    - 새로고침을 했을 때 페이지가 안뜸
    - 검색엔진에서 사용
  - HashRouter
    - Build, Delpoy시 편리함
    - 새로고침을 했을 때 브라우저에 물어봄
    - 관리자페이지에서 사용
- withRouter
- Switch
  - 해당하는 첫 번째 페이지를 보여준다.
  - 동시에 여러 개의 router가 보여지는 것을 막아준다.

## React Bootstrap

```js
// 추가해야 함.
// Importing the Bootstrap CSS
import "bootstrap/dist/css/bootstrap.min.css";
```

## React helmet

- 웹 사이트의 head를 쉽게 수정할 수 있다.

## Deploy

### 1) Deploying to Github Pages

```bash
npm i gh-pages
or
yarn add gh-pages
```

1. package.json -> "homepage": "./" 추가
2. npm run build 실행
3. package.json -> "homepage": "https://hgko1207.github.io/{repository}/" 변경
4. package.json -> "scripts" -> "deploy": "gh-pages -d build" 추가
5. npm run deploy 실행

### 2) Deploying to Heroku

- Heroku는 간단하게 무료로 호스팅 할 수 있도록 해주는 서비스이다.

- package.json 안에 아래 내용을 추가한다.

```json
"heroku-postbuild": "npm install && npm install --only=dev --no-shrinkwrap && npm run build"
```

- [Heroku 사이트](https://dashboard.heroku.com/)를 접속하여 계정을 생성하고 로그인한다.
- **create a new app** 한 후 Deploy 탭을 선택한다.
- GitHub 계정을 연결 한 후 Manual deploy 한다.

### 3) Deploying to Netlify

- [Netlify](https://www.netlify.com/)는 GitHub, GitLab 등과 계정 연동 및 쉬운 호스팅을 제공한다.

#### GitHub 연동

- 사이트를 접속하여 GitHub와 연결하여 Sign-up(회원가입)을 합니다.
- 로그인 후 **New site from Git** 버튼을 클릭합니다.
-

## ES6 문법

- Class
- import
- map
- filter
- fill
- reduce

## 알아두면 좋은 것

- Node는 자바스크립트 실행기이다. (백엔드, 서버가 아님)
- Node에서는 require 사용
- Hooks는 함수 컴포넌트가 전체로 재실행되는 현상이 있다.

## 강의자료

- [ZeroCho TV - React 기본 강좌 1-1. 리액트를 왜 쓰는가](https://www.youtube.com/watch?v=V3QsSrldHqI&list=PLcqDmjxt30RtqbStQqk-eYMK8N-1SYIFn)
- [Nomad Coders Academy](https://academy.nomadcoders.co/courses/category/KR)
- [Inflearn](https://www.inflearn.com/)

## 공식문서

- [React 시작하기](https://ko.reactjs.org/docs/getting-started.html)
- [React Training / React Router](https://reacttraining.com/react-router/web/api/matchPath/returns)

## 참고자료

- [자그마한 리액트 팁 모음](https://react-etc.vlpt.us/)
- [React 강좌) trendy React 0-0. 개요](https://velog.io/@public_danuel/trendy-react-0-0)
