## 회원 + 게시글 프로젝트

#### ♟️ 구조
- MVC
- Dao(Data Access Object): DB의 데이터에 접근하기 위한 객체, 직접 DB에 접근, 데이터 삽입, 삭제, 조회
- Dto(Data Transfer Object): 계층 간 데이터 교환은 위함, 로직을 가지지 않는 데이터 객체, getter/setter 메소드만 가짐

#### 📝 게시글 (명언앱과 비슷한 기능 + 로그인 후 사용 가능한 서비스)

![image](https://github.com/ohyo555/23_12_AM/assets/153146836/5cf1cb06-c9b1-413a-a828-15989003339a)
- 작성
- 목록
- 상세보기
- 수정, 삭제: 로그인한 사용자이면서 작성자에 한해서 가능한 기능

#### 🙎🏻‍♀️ 회원 🙎🏻‍♂️
![image](https://github.com/ohyo555/23_12_AM/assets/153146836/1c0a1ae4-f3ad-413e-8a71-fa79a8462e02)
- 전역에서 member를 관리시켜서 로그인한 경우 member를 변경하고 로그아웃 시에는 member를 null 처리
    * 회원가입: 이미 회원가입된 아이디에 대한 확인
    * 로그인: 현재 로그인 중인 사용자가 있는지 확인, 회원가입된 아이디와 비밀번호의 일치 확인
    * 로그아웃: 로그인된 member를 null처리

