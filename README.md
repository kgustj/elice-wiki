# elice-wiki

> 엘리스 AI 트랙 4기 · 팀 미니 프로젝트 · 2022.04 ~ 06

엘리스 수강생이 커리큘럼에 따라 학습 기록을 남기고, 공유하고, 토론하는 위키형 커뮤니티 서비스입니다.

> 최신 코드는 [`feature-board-front`](https://github.com/kgustj/elice-wiki/tree/feature-board-front) 브랜치에 있습니다. `dev` 브랜치의 내용도 모두 포함합니다.

## 내 역할: 프론트엔드

홈, 헤더, 검색, 관리자 페이지, 마이페이지 화면을 맡았습니다. 프론트엔드 커밋 기록에서 추가한 줄 수로 팀 내 2위입니다 (4,270줄).

- **홈 최근 게시물**: 최근 게시물 목록 ([`RecentList`](https://github.com/kgustj/elice-wiki/blob/feature-board-front/front/src/components/view/home/RecentList.js))
- **헤더**: 메뉴, 로그아웃 ([`Header`](https://github.com/kgustj/elice-wiki/blob/feature-board-front/front/src/components/view/Header.js))
- **검색 기능** ([`Search`](https://github.com/kgustj/elice-wiki/blob/feature-board-front/front/src/components/view/home/Search.js))
- **관리자 페이지**: 페이지 구성과 라우팅을 시작했고, 이후 hongloans 님이 이어서 작업 ([`admin`](https://github.com/kgustj/elice-wiki/tree/feature-board-front/front/src/components/admin))
- **마이페이지·유저 카드** ([`mypage`](https://github.com/kgustj/elice-wiki/tree/feature-board-front/front/src/components/mypage))
- **UI 라이브러리 전환**: antd에서 MUI로 변경, Prettier 설정

## 주요 기능

- 커리큘럼별 학습 기록(게시글) 작성과 공유, 마크다운 에디터
- 댓글과 토론
- 최근 게시물, 검색
- 회원가입, 로그인, 마이페이지
- 관리자 페이지

## 기술 스택

| 구분 | 사용 기술 |
|---|---|
| Frontend | React, MUI, styled-components, Recoil, Redux, Toast UI Editor |
| Backend | Node.js, Express, MySQL(Sequelize), JWT, AWS SDK |

## 팀 구성

커밋 기록 기준으로 각자 주로 작업한 부분입니다. 이름 대신 GitHub 아이디로 적었습니다.

| 팀원 | 담당 | 주로 작업한 부분 |
|---|---|---|
| **Kim-Hyunseo (김현서)** | 프론트엔드 | 홈 최근 게시물, 헤더, 검색, 관리자·마이페이지 |
| songgaram | 프론트엔드 | 화면 전반, 로그인 |
| hongloans | 프론트엔드·백엔드 | 관리자·마이페이지, 회원 API |
| violetwhenisawu | 프론트엔드 | 화면, 노트 |
| nowgnas (sangwon) | 백엔드 | 백엔드 전반, 게시글 API, DB 모델 |
| KA | 백엔드 | 게시판·댓글 API, DB 모델 |

## 실행

```bash
git checkout feature-board-front
cd back && npm install && npm start     # MySQL 접속 정보가 담긴 .env 필요
cd front && npm install && npm start
```

## 저장소 안내

팀 GitHub 저장소(elice-mini-project/elice-wiki)를 커밋 기록과 브랜치 그대로 옮겨 온 사본입니다. 접속 정보가 담긴 `.env` 파일은 커밋 기록에서 지웠습니다.
