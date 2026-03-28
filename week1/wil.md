1주차 학습 내용 요약


1. 웹(Web)의 동작 원리
클라이언트-서버 구조: 웹은 요청(Request)을 보내는 '클라이언트'와 요청을 처리해 응답을 주는 '서버' 간의 소통으로 이루어짐.

URL (Uniform Resource Locator): 웹상에서 특정 자원(페이지, 이미지 등)의 위치를 나타내는 주소 체계입니다. 스킴(http/https), 호스트(도메인), 포트, 패스, 쿼리 파라미터 등으로 구성됨.


2. HTTP 프로토콜
정의: 클라이언트와 서버가 데이터를 주고받기 위한 통일된 규칙

특징: 서버가 이전 상태를 기억하지 않는 무상태성과 응답 후 연결을 끊는 비연결성을 가짐.

주요 메서드 :

GET: 리소스 조회

POST: 새로운 리소스 생성

PUT/PATCH: 리소스 수정 (전체 수정/일부 수정)

DELETE: 리소스 삭제

상태 코드 (응답 결과): 200(성공), 201(생성 성공), 400(잘못된 요청), 404(찾을 수 없음), 500(서버 오류) 등.



3. REST API 
API: 프로그램 간 소통을 위해 미리 정해놓은 약속

REST API: HTTP의 장점을 최대한 활용하는 아키텍처 스타일

구성 요소: 자원(URI), 행위(HTTP 메서드), 표현(JSON 등).



4. 프론트엔드 vs 백엔드
프론트엔드: 사용자가 직접 보고 상호작용하는 UI를 개발하며, 서버에서 받은 데이터를 화면에 그리는 역할을 합니다.

백엔드: 눈에 보이지 않는 영역에서 비즈니스 로직을 처리하고, "데이터베이스(DB)"에 데이터를 저장 및 관리하며 클라이언트의 요청에 응답함.



5. 스프링 부트 (Spring Boot)
자바 기반의 대규모 애플리케이션 프레임워크인 '스프링'을 복잡한 설정 없이 쉽고 빠르게 사용할 수 있도록 도와주는 도구. 이번 스터디에서 주로 사용하게 될 도구임.


/////////////////////////////////////////////////////////////////


온라인 쇼핑몰 프로젝트 API 명세서 작성

- 상품 기능

1. 상품 정보 등록
   HTTP Method: POST
   URI: /goods

2. 상품 목록 조회
   HTTP Method: GET
   URI: /goods

3. 개별 상품 정보 상세 조회
   HTTP Method: GET
   URI: /goods/{goodsId}

4. 상품 정보 수정
   HTTP Method: PATCH
   URI: /goods/{goodsId}

5. 상품 삭제
   HTTP Method: DELETE
   URI: /goods/{goodsId}




- 주문 기능

1. 주문 정보 생성
   HTTP Method: POST
   URI: /orders

2. 주문 목록 조회
   HTTP Method: GET
   URI: /orders

3. 개별 주문 정보 상세 조회
   HTTP Method: GET
   URI: /orders/{orderId}

4. 주문 취소
   HTTP Method: DELETE
   URI: /orders/{orderId}


//////////////////////////////////////////////////////

Spring Boot 애플리케이션을 실행하고, 브라우저에 localhost:8080 을 입력했을 때 나오는 Whitelabel Error Page 스크린샷






///////////////////////////////////

