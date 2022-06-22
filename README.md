# -1
3/21 프젝 수업1
프로젝트명 : 매입 매출 자료 확인
이클립스를 통해 자바로 프로젝트를 구현할 생각입니다!
어떤 회사에서 어떤 물건이 얼마에 들어오고 어디로 얼마에 나가는지
개수가 어떻게 되는지 그런 것들을 구현할 생각입니다.

※ 초안 단계라고 생각해서 주제를 바꿀 수도 있습니다!

ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

4/4
개체 : 내 회사, 업체, 부품, //신고(소득세? 같은 것들)
내 회사 : 회사명, 이름, ...
업체 : 업체명, 업체원, ...
부품 : 부품명, 재고, ...
//신고 : 소득세, 신고일, ....
관계 : 구매, 판매, 요청(?)
구매 : 구매일자, 수량, 금액, 부가세(?)..
판매 : 판매일자, 수량, 금액, 부가세(?)..

※ 대강 머릿속으로 그림은 그려지는데 표현해내기는 어려운 것 같습니다..
  계속해서 생각해보면서 틀을 잡아보려고 합니다.
  이클립스로 자바로 하려고 했는데 C#으로 만들어볼까 생각도 듭니다.
  아니면 아예 다른 주제로 해버릴까.. 생각도 듭니다.
  부족하게 해서 죄송합니다 ㅜㅜㅜ
  
  ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
5/16
※ 기존에 하려던 것이 구상해봤을 때 테이블 한 개 정도 밖에는 안나오고 과제로 해내기에는 별로인 것 같아서 다시 구상해서 올립니다ㅜㅜ
주제 : 전국의 동물 병원을 검색해서 병원에 대한 정보를 얻고, 병원에 대한 정보를 사용자들이 직접 등록해서 공유할 수 있는 서비스

<요구사항 명세서>
1. 애니멀 케어에 회원으로 가입하려면 회원 아이디, 비밀번호, 이름, 나이, 회원 주소를 입력해야한다.
2. 회원은 회원 아이디로 식별한다.
3. 회원 주소는 하나만 가질 수 있다.
4. 병원은 병원 이름, 병원 주소, 병원 연락처, 별점 정보를 유지해야 한다.
5. 병원은 병원 연락처로 식별한다.
6. 병원 주소는 하나만 가질 수 있다.
7. 병원 별점의 초기 값은 0.0이다.
8. 상품에 대한 상품번호, 상품명, 재고량, 단가 정보를 유지해야 한다.
9. 상품은 상품번호로 식별한다.
10. 회원은 여러 상품을 주문할 수 있고, 하나의 상품을 여러 회원이 주문할 수 있다.
11. 회원이 상품을 주문하면 주문에 대한 주문번호, 주문수량, 배송지, 주문일자 정보를 유지해야 한다.
12. 각 상품은 한 제조업체가 공급하고, 제조업체 하나는 여러 상품을 공급할 수 있다.
13. 제조업체가 상품을 공급하면 공급일자와 공급량 정보를 유지해야 한다.
14. 제조업체에 대한 제조업체명, 전화번호, 위치, 담당자 정보를 유지해야 한다.
15. 제조업체는 제조업체명으로 식별한다.
16. 회원은 여러 병원 정보를 등록할 수 있고, 하나의 병원은 한 명의 회원만 등록할 수 있다.
17. 등록에 대한 병원 이름, 주소, 연락처, 별점 정보를 유지해야한다.
18. 회원은 여러 병원의 리뷰를 작성할 수 있고, 리뷰 하나는 한 명의 회원만 작성할 수 있다.
19. 작성에 대한 리뷰 번호, 병원 번호, 작성자(회원 아이디), 글 제목, 글 내용, 작성 일자, 별점 정보를 유지해야한다.
20. 리뷰는 리뷰 번호로 식별한다.
21. 회원은 여러 리뷰의 댓글을 달 수 있고, 댓글 하나는 한 명의 회원만 달 수 있다.
22. 댓글달기에 대한 댓글 번호, 리뷰 번호, 작성자(회원 아이디), 댓글 내용을 유지해야한다.
23. 댓글은 댓글 버너호로 식별한다.
24. 회원은 즐겨찾기는 병원을 추가할 수 있다.
25. 즐겨찾기는 즐겨찾기 아이디로 식별한다.

개체 - 회원, 병원, 상품, 제조업체, 리뷰, 댓글, 즐겨찾기
속성 - 회원 아이디, 비밀번호, 이름, 나이, 주소, 병원 연락처, 병원 이름, 병원 주소, 별점, 상품 번호, 상품명, 재고량, 단가, 공급일자, 공급량, 제조업체명, 전화번호, 위치, 담당자, 주문 번호, 주문 수량, 배송지, 주문일자, 리뷰 번호, 병원 번호, 회원 아이디, 글 제목, 글 내용, 작성 일자, 별점, 댓글 번호, 리뷰 번호, 회원 아이디, 댓글 내용, 즐겨찾기 아이디, 회원 아이디, 병원 연락처
관계 - 등록, 주문, 공급, 작성, 댓글달기, 추가

E-R 다이어그램
<img width="572" alt="er다이어그램" src="https://user-images.githubusercontent.com/81346079/169820539-3ccac0c8-164f-402b-b9d3-03e71bc29af7.png">

릴레이션 스키마
<img width="318" alt="릴레이션스키마" src="https://user-images.githubusercontent.com/81346079/169823143-43d091f6-e547-48f0-8113-75dd9b73b572.png">
*주문에 상품번호도 밑줄

<개체와 속성 추출> 개체(??) - 속성(??, ??, ...)
회원 - 회원 아이디(키 속성), 비밀번호, 이름, 나이, 주소
병원 - 병원 연락처(키 속성), 병원 이름, 병원 주소, 별점
상품 - 상품번호(키 속성), 상품명, 재고량, 단가
리뷰 - 리뷰 번호(키 속성), 병원 번호, 회원 아이디, 글 제목, 글 내용, 작성 일자, 별점
댓글 - 댓글 번호(키 속성), 리뷰 번호, 회원 아이디, 댓글 내용
즐겨찾기 - 즐겨찾기 아이디(키 속성), 회원 아이디, 병원 연락처

<개체 간의 관계> 관계(??) - 관계에 참여하는 개체 - 관계 유형 - 속성
등록 - 회원(선택) / 병원(필수) - 관계 유형(1:n) - 
작성 - 회원(선택) / 리뷰(필수) - 관계 유형(1:n) -
주문 - 회원(선택) / 상품(선택) - 관계 유형(n:m) - 주문번호, 주문수량, 배송지, 주문일자
댓글달기 - 회원(선택) / 댓글(필수) - 관계 유형(1:n) - 
추가 - 회원(선택) / 즐겨찾기(필수) - 관계 유형(1:n) - 

<테이블 생성 스크립트>
create table 회원(
회원아이디 varchar(100) not null,
비밀번호 varchar(100) not null,
이름 varchar(100) not null,
나이 int,
회원주소 varchar(100) not null,
primary key(회원아이디)
);

create table 병원(
병원연락처 varchar(100) not null,
회원아이디 varchar(100) not null,
병원이름 varchar(100) not null,
병원주소 varchar(100) not null,
별점  varchar(100) not null default 0,
primary key(병원연락처),
foreign key(회원아이디) reference 회원(회원아이디)
);

create table 즐겨찾기(
즐겨찾기번호 int(100) not null auto_increment,
회원아이디 varchar(100) not null,
병원연락처 varchar(100) not null,
primary key(즐겨찾기번호),
foreign key(회원아이디) reference 회원(회원아이디),
foreign key(병원연락처) reference 병원(병원연락처)
);

create table 리뷰(
리뷰번호 int not null,
회원아이디 varchar(100) not null,
병원연락처 varchar(100) not null,
글제목 varchar(100) not null,
글내용 varchar(300) not null,
별점 varchar(100) not null,
primary key(리뷰번호),
foreign key(회원아이디) reference 회원(회원아이디),
foreign key(병원연락처) reference 병원(병원연락처)
);

create table 댓글(
댓글번호 int not null auto_increment,
회원아이디 varchar(100) not null,
리뷰번호 int not null,
댓글내용 varchar(100) not null,
primary key(댓글번호),
foreign key(회원아이디) reference 회원(회원아이디),
foreign key(리뷰번호) reference 리뷰(리뷰번호)
);

create table 상품(
상품번호 int not null auto_increment,
상품명 varchar(100) not null,
재고량 int not null default 0,
단가 int,
제조업체명 varchar(100) not null,
공급일자 varchar(100),
공급량 int not null default 0,
primary key(상품번호),
foreign key(제조업체명) reference 제조업체(제조업체명)
);

create table 제조업체(
제조업체명 varchar(100) not null,
전화번호 varchar(100) not null,
위치 varchar(100) not null,
담당자 varchar(100) not null,
primary key(제조업체명),
);

create table 주문(
회원아이디 varchar(100) not null,
상품번호 int not null auto_increment,
주문번호 int
주문수량 int
배송지 varchar(100) not null,
주문일자 varchar(100) not null,
foreign key(회원아이디) reference 회원(회원아이디),
foreign key(상품번호) reference 상품(상품번호)
);

5/23 테이블 생성 스크립트 부분이 아직 미흡한 부분도 있는 것 같고 놓치고 넘어간 부분도 있을 것 같습니다. 좀 더 신경을 써보고 추후에 수정해보도록 하겠습니다!

5/28
제1 정규화
초기 릴레이션에선 즐겨찾기 리스트의 병원 연락처가 아래와 같이 다중 값 속성을 포함하고 있었음
<img width="353" alt="1차 정규화" src="https://user-images.githubusercontent.com/81346079/170814855-e88a2748-91b9-4148-862f-c9725882d857.PNG">
-회원 릴레이션 중 일부 속성

<img width="353" alt="1차 정규화2" src="https://user-images.githubusercontent.com/81346079/170814857-e6710740-1c45-4aad-902a-ca7a1d256d02.PNG">
1차 정규형에 속하게 바꿈

제2 정규화
회원 릴레이션이 1차 정규형은 만족했지만 데이터 중복으로 인한 이상 현상이 발생함. 회원 릴레이션에 즐겨찾기 아이디가 기본 키에 포함 되어 있어서 즐겨찾기를 등록하지 않은 회원은 삽입 불가. 또한 즐겨찾기를 삭제해서 관련 튜플을 삭제하게 되면 즐겨찾기와 관련이 없는 회원 아이디, 비밀번호, 등 회원 관련 데이터까지 손실됨. 원인을 알아보기 위해 회원 릴레이션의 함수 종족 다이어그램을 그려봄.

<img width="174" alt="2차 정규화1" src="https://user-images.githubusercontent.com/81346079/170814873-f30e669f-1025-4a05-b0b2-274726122ce5.PNG">
- 회원 릴레이션의 함수 종속 다이어그램

그림을 참고하면, 원인은 기본키에 완전 함수 종속되지 못한 비밀번호, 회원이름, 나이, 회원주소때문. 부분 함수 종속이 제거되도록 회원 릴레이션을 분해해서 2차 정규형에 속하게 바꿈

<img width="237" alt="2차 정규화2" src="https://user-images.githubusercontent.com/81346079/170814925-936e5662-4638-405f-bc05-5abd9b19fc94.PNG">
- 회원 릴레이션과 즐겨찾기의 함수 종속 다이어그램

제3 정규화
릴레이션이 제2 정규형에 속했고, 기본키가 아닌 모든 속성이 기본키에 이행적 함수 종속이 되어 있지 않아서 별 다른 절차없이 제3 정규형을 만족하는 상태가 됨.

<img width="115" alt="3차 정규화1" src="https://user-images.githubusercontent.com/81346079/170816023-51688391-2fe6-4073-ae22-264da6a67cd3.PNG">
- 회원 릴레이션의 함수 종속 다이어그램

<img width="112" alt="3차 정규화2" src="https://user-images.githubusercontent.com/81346079/170816040-6bf8fe46-2062-42d6-ace5-41a7bfa38e3f.PNG">
- 병원 릴레이션의 함수 종속 다이어그램

<img width="110" alt="3차 정규화3" src="https://user-images.githubusercontent.com/81346079/170816101-97e97b5f-2fa9-46b7-853c-ed211ede439e.PNG">
- 리뷰 릴레이션의 함수 종속 다이어그램

------------------------------------------
6/23

테이블 수정이 있어서 6/23일 기준으로 다시 올립니다.

create table member(
id varchar(100) not null,
pwd varchar(100) not null,
name varchar(100) not null,
phone varchar(100) not null,
adress varchar(100) not null,
primary key(id));

create table hospital(
hosphone varchar(100) not null,
hosname varchar(100) not null,
hosadress varchar(100) not null,
primary key(hosphone));

create table favorite(
favnum int(100) not null auto_increment,
id varchar(100) not null,
hosphone varchar(100) not null,
primary key(favnum),
foreign key(id) references member(id),
foreign key(hosphone) references hospital(hosphone));

create table review(
revnum int not null auto_increment,
id varchar(100) not null,
hosphone varchar(100) not null,
title varchar(100) not null,
revcontent varchar(300) not null,
primary key(revnum),
foreign key(id) references member(id),
foreign key(hosphone) references hospital(hosphone));

create table comment(
comnum int not null auto_increment,
id varchar(100) not null,
prodname varchar(100) not null,
comcontent varchar(100) not null,
primary key(comnum),
foreign key(id) references member(id)
);

create table product(
prodnum int not null auto_increment,
prodname varchar(100) not null,
stock int not null default 0,
price int,
manname varchar(100) not null,
prodatestock varchar(100),
primary key(prodnum),
foreign key(manname) references manufacturer(manname));

create table manufacturer(
manname varchar(100) not null,
manphone varchar(100) not null,
manadress varchar(100) not null,
person varchar(100) not null,
primary key(manname));

create table orderlist(
ordernum int not null auto_increment,
id varchar(100) not null,
prodname varchar(100) not null,
quantity int,
adress varchar(100) not null,
orderdate varchar(100) not null,
primary key(ordernum)
);

