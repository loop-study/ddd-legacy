# 키친포스

## 요구 사항
간단한 식당 관리 앱을 구현한다.
메뉴와 상품, 주문(배달, 포장, 취식), 테이블로 구성된다.

### 메뉴 그룹
- [x] 사용자가 보는 메뉴그룹을 생성한다.
    - [x] 메뉴그룹명은 반드시 한글자 이상 입력해야 한다.
    - [x] 메뉴그룹명은 중복이 가능하다.
- [x] 등록된 메뉴그룹 내역을 확인할 수 있다.
  
### 메뉴
- [x] 사용자가 보는 메뉴를 생성한다.
    - [x] 메뉴는 메뉴그룹에 포함된다.
    - [x] 메뉴에는 상품이 1개 이상 포함되어야한다.
    - [x] 메뉴의 가격은 포함된 상품가격보다 높을 순 없다. 
    - [x] 상품 수량은 1개 이상이어야 한다. 
- [x] 등록된 메뉴를 숨길 수도 보일 수도 있다.
- [x] 등록된 메뉴의 가격은 변경이 가능하다.
- [x] 등록된 메뉴 내역을 볼 수 있다. 

### 상품
- [x] 상품을 추가할 수 있다.
    - [x] 상품은 상품명과 가격으로 이뤄진다.
    - [x] 상품명은 중복이 가능하다.
    - [x] 상품명은 한글자 이상 가능하다.
    - [x] 가격은 0원 이상만 입력이 가능하다
- [x] 등록된 상품의 가격을 변경할 수 있다. 
    - [x] 변경된 상품이 포함된 메뉴의 가격이 해당 메뉴의 상품들의 가격보다 높으면 비노출한다.   
- [x] 등록된 상품 내역을 확인할 수 있다.

### 테이블
- [x] 식당의 테이블을 관리한다.
    - [x] 테이블은 추가할 수 있다.
- [x] 손님이 입장하면 앉은 테이블을 활성화한다.
    - [x] 손님이 몇명인지 입력한다.
        - [x] 0명 미만은 안된다.
    - [x] 주문이 끝난 테이블이 초기화된다.
- [x] 식당 테이블 상황을 확인할 수 있다.

### 주문
- [ ] 주문은 배달, 포장, 취식으로 구분된다.
    - [ ] 공통
        - [ ] 주문타입에 관계없이 대기 상태로 시작된다.
        - [ ] 관리자가 대기상태의 주문을 접수한다.
        - [ ] 주문 메뉴와 주문 시간을 기록해야한다.
    - [ ] 배달
        - [ ] 배달 주문은 대기 -> 접수 -> 제공 -> 배달중 -> 배달됨 -> 완료로 단계가 진행된다.
        - [ ] 배달 받을 주소를 입력해야한다.
        - [ ] 주문 접수 시에 배달라이더에게 주문 정보(주문번호, 주문금액, 배송주송)를 전달한다.
    - [ ] 취식
        - [ ] 취식 주문은 대기 -> 접수 -> 제공 -> 완료로 단계가 진행된다.
        - [ ] 테이블 번호를 입력해야한다.
    - [ ] 포장
        - [ ] 포장 주문은 대기 -> 접수 -> 제공 -> 완료로 단계가 진행된다.
- [ ] 주문 내역을 확인할 수 있다.

## 용어 사전

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
|  |  |  |

## 모델링
