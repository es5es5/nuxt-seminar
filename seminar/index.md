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

- Middleware
  페이지나 레이아웃이 렌더링되기 전에 실행할 사용자 정의 함수를 정의

3. 라우팅
  - 동적 라우팅
  `/path1/path2/:id`
  `_id.vue`로 파일 네이밍

  - 중첩 라우팅

  directory
```
pages/
--| chungdahm/
-----| abc.vue/
-----| def.vue/
--| chungdahm.vue
```

.nuxt/router.js
```
{
  path: "/chungdahm",
  component: _b5b776fc,
  name: "chungdahm",
  children: [{
    path: "abc",
    component: _62cf8260,
    name: "chungdahm-abc"
  }, {
    path: "def",
    component: _7293c0f3,
    name: "chungdahm-def"
  }]
}
```

4. 예제
 - 기본적인 라우터 세팅
 - 동적으로 테마 컬러 적용하기
  `middleware` 를 이용해서 router 에 meta 데이터 넣는 것처럼 동작하기
 - 전체 css 적용하기
  `assets` `nuxt.config.js` 를 이용해서 전체 css 적용

5. 참고자료
 - [Nuxt.js 한글자료](https://develop365.gitlab.io/nuxtjs-0.10.7-doc/ko/guide/)
 - [Vue SSR 제대로 적용하기](https://zuminternet.github.io/vue-ssr/)
 - [어서와, SSR은 처음이지?](https://d2.naver.com/helloworld/7804182)