LoginExample API 문서
====================

이 문서에서는 LoginExample의 Api및 RestApi에 대한 내용을 다룹니다.


통신 방법
=======

클라이언트 -> 서버(Upstream)
------------------------
클라이언트와 서버가 통신할때에는 http 통신을 기본적으로 이용합니다.

클라이언트에서 서버로 데이터를 보낼때는 JSON.parse(string)을 이용하여 json을 Javascript Object로 변환하여 전송합니다.


서버 -> 클라이언트(Downstream)
--------------------------
반대로 서버에서 클라이언트로 데이터를 보낼때는 Javascript Object를 JSON.stringfy(object)를 이용하여 JSON으로 변환하여 res.send(object)로 클라이언트에 전송합니다.


인증
===

차후 추가 예정

HTTP Response 상태 코드
====================

서버에 전송되는 값들에 대한 http Response는 각각의 상태코드로 표시됩니다.

로그인 요청 들어왔을 시
------------------
GET / 304

로그인 성공했을 시
--------------
GET /login_success 400

로그인 실패 시
-------------
GET /login_fail 404


데이터베이스 스키마
================
이 node 서버의 데이터베이스 스키마를 다룹니다.

차후 추가 예정
