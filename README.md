# [오늘은 너네집](유튜브경로)

# 프로젝트 소개
## 프로젝트 요약
- **오늘의집**을 모티브로 하여 '오늘은 너네집'이라는 가상의 브랜드와 기획을 더해 cloning.
- **진행 기간**: 2021.06.21 ~ 07.02
- **기획 포인트**
1. '오늘은 너네집'이라는 가상의 브랜드에서, 집 인테리어 사진을 공유하는 플랫폼

## 팀원 소개
Front - 권오현, 김명준, 전건우
Back - 김정연, 배찬영, 장동국

## 메인 서비스
1. 카카오 소셜 로그인으로 가입할 수 있습니다.
2. 집 사진과 글을 피드처럼 올릴 수 있습니다.
3. 피드를 필터링, 무한스크롤로 구경할 수 있습니다.
4. 마이페이지에서 내가 올린 사진과 글을 볼 수 있습니다. 

# 적용 기술 및 구현 기능
## 기술 스택
- Front-End : React, React Router, Sass, Dompurify, React Daum Postcode, JavaScript, CRA
- Back-End : Python, Django, My SQL, AWS
- Communication Tool : Trello, Git, GitHub, Slack
## 구현 기능 상세
### 데이터 모델링(김정연, 배찬영, 장동국)
- (데이터 모델링 간단하게 시각화여 추가할 예정)
### 카카오 소셜 로그인 (김정연)
1. 카카오 REST API를 이용하여 카카오 로그인 & 회원가입
2. 닉네임이 중복일 경우, 닉네임 추천 기능
3. 회원가입 성공 시, 가입 축하 메일 발송
4. 로그인 & 회원가입 성공시, JWT 발행
5. 회원 전용 서비스에 대해, JWT를 통한 인증과정을 데코레이터 함수로 구현
### 게시글 리스트 페이지 (배찬영)
1. 형태,스타읻 등 키워드로 필터링
2. 역대인기순,최신인기순 등으로 정렬
3. 무한 스크롤 형식의 페이지네이션
### 게시글 상세 페이지 (장동국)
1. 게시글 상세 데이터 조회
### 댓글 , 좋아요 (장동국)
2. 댓글 C.R.U.D 및 페이지네이션
2. 찜하기 C.R.U.D
### 게시글 작성 페이지 (배찬영)
1. AWS를 활용 - 사진을 S3에 업로드 & RDS DB에서 URL 활용 
### 마이 페이지 (김정연)
1. 유저의 게시글 & 찜하기 데이터 조회

# Reference
1. 이 프로젝트는 [오늘의 집]https://ohou.se/를 참조하여 학습 목적으로 만들었습니다.
2. !!개발 클론이 아닌 '기획 클론'
오늘은 너네집 프로젝트는 오늘의 집 클론 프로젝트이지만, 백지 상태에서 구현되었습니다.
개발자의 역할은 기획이 아닌, 기획 의도를 현실로 바꾸는, 기획의 ‘구현’이라 생각합니다.
따라서, 기획 과정을 건너 뛰고 구현에 집중하기 위해 오늘의 집 이라는 서비스를 참고한 것일 뿐,
프로젝트의 모든 기능은, 실제 서비스 개발과정과 마찬가지로, 백지 상태에서 구현되었음을 밝힙니다.
3. 프로젝트에 사용한 모든 이미지와 영상은 저작권에 문제가 없는 컨텐츠를 사용하여 만들었습니다.
4. 실무 수준의 프로젝트이지만 학습용으로 만들었기 때문에 이 코드를 활용하여 이득을 취하거나 무단 배포할 경우 법적으로 문제될 수 있습니다.
