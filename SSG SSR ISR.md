### pre-render
- 페이지가 사용자에게 전해지기 전에 HTML을 미리 생성하고 구성하는 방식

### SSG
- 정적 사이트 생성(Static Site Generation)
- getStaticProps

### SSR
- 서버사이드 렌더링(Server Side Rendering)
- 유저가 브라우저를 통해 사이트에 접속하면 사이트 서버에서 렌더링에 필요한 데이터를 유저 쪽으로 보내주는 방식이다.
- SEO에 좋다
- 사용자가 많고, 데이터 정보가 클수록 서버 부담이 과중된다.
- getServerSideProps

### ISR
- 빌드 시에만 정적 페이지를 생성하는 것이 아니라 특정 시간(초)마다 정적 페이지를 재생성하는 방식
- getStaticProps의 revalidate 값을 준다