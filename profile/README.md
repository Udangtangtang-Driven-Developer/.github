# 스파게티 코드

### 기획 의도

#### 문제 인식

개발자들끼리 코드를 넘어 설계, 테스트 등 다양한 영역에서 서로 리뷰를 하고 의견을 나눌 수 있는 놀이터가 있었으면 좋겠다.

### 기능 브레인 스토밍

- 회원

  - 내가 쓴 글 조회
  - 내가 쓴 코멘트 조회
  - 로그인
    - jwt 방식 (Access token, Refresh token)

- 게시글

  - 게시글 구성

    - 제목
    - 본문 (컬러 적용 가능 마크 다운)
    - 태그
    - 컬러
    - 커버 이미지 (optional)

  - 리스트 조회

    - 태그별, 최신 순, 조회 순

  - 등록

    - 미리보기
    - 임시 저장 기능
    - 공개 여부 선택
    - 맞춤법 (optional)

  - 삭제
  - 수정

- 리뷰 코멘트 (실시간)

  - 등록
    - 컬러 적용 마크 다운 지원
  - 수정
  - 삭제
  - 유저 태그 (글로벌 검색 - 일단은 RDBMS like만 사용)

- 알림 (실시간)
  - 내가 쓴 게시글 코멘트 등록 시 알림
  - 코멘트에 태깅 시 알림
---
Phase 1 기능 구현 계획
<img width="911" alt="image" src="https://github.com/Udangtangtang-Driven-Developer/.github/assets/22143650/98b84368-ef2e-43c9-a6e7-a1c7b820ade1">



### 활용 기술
- Backend : Nest.js, Prisma
- Frontend : Next.js
