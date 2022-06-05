# 기능 요구 사항

# 회원가입

- [ ]  email, password, nickname을 받아 회원 정보를 등록한다.
   - [x]  email 중복 검증
   - [x]  email 규칙 검증
   - [x]  password 규칙 검증
   - [x]  nickname 규칙 검증
   - [ ]  누락 정보 검증
   - [x]  데이터베이스에 저장

# 로그인(토큰 기반)

- [x]  email, password를 받아 로그인을 할 수 있다.
   - [x]  email, password가 db에 저장된 값과 일치하는지 검증
   - [x]  jwtToken을 생성
   - [x]  nickname과 token을 response로 반환

# 회원 정보

## 회원 정보 식별

- [x]  token으로 회원을 식별하여 db에서 회원을 가져온다.

## 회원 정보 조회

- [x]  비밀번호를 검증한다.
- [x]  email, nickname을 응답한다.

## 회원 정보 수정

- [x]  nickname을 수정할 수 있다.
- [x]  password를 수정할 수 있다.

nickname와 password는 회원 가입 시와 같은 조건으로 검증한다.

## 회원 탈퇴

- [x]  db에서 해당 회원 정보를 삭제한다.