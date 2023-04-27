
#잇츠미 eatsMe

####주소
eatsme.site

####소개
잇츠미(eatsMe)는 식도락 여행을 기반으로한 정보 공유 및 커뮤니티 기능을 가지고 있습니다.
자신만의 맛집 코스를 공유하거나, 선택한 지역의 인기있는 맛집을 보여주는 서비스를 제공합니다.

####기능 요약

1. 웹 사이트 이용자가 자신이 알고있는 좋은 맛집 코스를 작성, 공유하고 다른 이용자들과 소통, 정보 공유를 목적으로 하는 커뮤니티 기능을 가집니다.
2. 웹 사이트 이용자가 작성한 맛집들을 데이터로 쌓고, 이 데이터와 함께 구글 API에서 평점 높은 맛집들을 받아 선택한 지역의 인기있는 맛집을 제공합니다.

####개발 기간
2023년 3월 10일 ~ 2023년 4월 5일

#### 기술

- HTML, CSS, JavaScript, TypeScript, React, Next.js, GraphQL, Rest-API

- T-map, AWS

#### 기술 선택 이유

- React
  리액트의 Virtual DOM 기능으로 실제 DOM으로 적용하기 전에 가상 DOM을 만들어 최종 완성된 결과만을 전달하기 때문에 브라우저의 연산양을 줄여 성능을 개선시켜서 좋고, 코드의 재사용성이 높기 때문에 사용하였습니다.

- TypeScript
  명시적인 정적타입으로 컴파일 단계에서 오류를 포착하여 코드의 가독성을 높여 디버깅이 쉽기 때문에 선택하였습니다.

- GraphQL
  구체적이고 정확하게 받아오고 싶은 데이터만 가져올 수 있으므로 불필요한 Over-fetching을 해결하였습니다.

- Rest-API
  모든 정보가 필요한 페이지에서는 굳이 GraphQL 방식이 아닌 Rest-API를 사용하여 데이터를 편하게 불러오도록 했습니다.

- T-Map

#### 구현 기능

게시글(맛집 코스) 작성 / 수정 / 삭제 / 조회

- 게시글 작성시 작성한 좌표마다 맵의 마커가 찍히고, 경유지가 추가될 때마다 전체 경로를 보여줍니다.
- 게시글 목록에서 게시글 조회시 해당 게시글의 코스(좌표)에 따른 마커가 맵에 표시되며 마커를 눌러 추가적인 작업이 가능합니다.

예약

- 게시글 목록의 맵에 찍힌 마커(좌표)를 눌러 해당 식당 정보를 받아 예약페이지로 이동됩니다.
  받아 온 식당 정보에 날짜와 시간을 선택하면 예약됩니다.

맛집 목록

- 구글 API를 활용한 데이터를 Rest-API 방식을 사용하여 선택 지역의 평점 높은 식당들의 정보를 불러옵니다.

마이페이지

- 내가 쓴 글, 찜한 게시글(코스), 예약 내역을 확인할 수 있습니다.

로그인 / 회원가입 / 권한분기

- 이메일 인증을 통한 회원가입이 가능하고, 특정 페이지에서 로그인 권한분기 처리가 되어있습니다.

####멤버 구성

- 박선우 (팀장,BE)
- 김병수 (FE)
- 전은찬 (FE)
- 최민기 (FE)
- 김진겸 (BE)
- 김재윤 (BE)
- 이상언 (BE)
