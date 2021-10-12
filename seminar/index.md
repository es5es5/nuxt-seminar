1. 설치
```bash
using NPM
$ npm install -g @vue/cli @vue/cli-init // Vue CLI 설치

$ npm init nuxt-app <Project>
```

2. 디렉토리 구조

- Layouts
 전체 레이아웃 `<Nuxt></Nuxt>` 태그에 Pages 이하 컴포넌트들이 라우팅 되서 들어옴
 /Pages 에서 

- Pages
 <b>Nuxt 와 Vue 의 가장 크게 다른 점이라고 생각함</b>
 /Pages 에 `.vue` 파일을 넣으면 자동으로 라우팅 설정

    - 동적 라우팅
    `/path1/path2/:id`
    `_id.vue`로 파일 네이밍

- Middleware
  페이지나 레이아웃이 렌더링되기 전에 실행할 사용자 정의 함수를 정의

3. 라우팅
