# GYM database system - DBMS project 2018
基於mysql的資料庫查詢系統，用來管理健身房

## Diagrams
### ER Diagram
![ER](./diagrams/ER.PNG)
#### Attribute
* **member**:健身房的學員
  * MNUMBER:學員的編號
  * MNAME:學員的名字
  * PHONE:學員的手機
  * AGE:學員的年齡
* **trainer**:健身房的教練
  * TNUMBER:教練的編號
  * TNAME:教練的名字
  * EXPERIENCE:教練的教學資歷
  * WORKHOUR:教練的上班時間
* **proposal**:方案
  * PNAME:方案的名稱
  * DEADLINE:方案的使用期限
  * PRICE:方案的價錢
  * MEMBERSHIP:是否需繳入會費
* **course**:課程
  * CNUMBER:課程的編號
  * CNAME:課程的名稱
  * PEOPLELIMIT:課程的人數上限
* **branch**:健身房的分店
  * BNAME:分店名稱
  * AREA:分店所在的區域
  * OPENHOUR:分店的營業時間
#### Relationship
* trainer **INSTRUCT** member:每個教練可以指導很多學員，但每個學員一定要有教練且只能有一個
* member **ENROLL** proposal:每個學員一定要報名方案且只能報名一種，但每種方案可以有很多學員報名且一定有人報名
* member **INQUIRE** proposal:每個學員一定會詢問很多個方案，而且每個方案一定也有很多個學員詢問
* member **APPLY** course:每個學員可能會報名很多個課程，但不一定每個人都會報名課程，每個課程一定會有很多學員報名
* branch **HAVE** course:每個分店一定擁有很多個課程，而且每種課程一定被很多個分店擁有
* trainer **TEACH** course:每個教練可能教很多個課程，但不一定每個教練都有教，但每個課程一定有教練教學
* member **BELONG** branch:每個學員一定屬於某個分店，而且每個分店一定有很多個學員
* trainerer **BELONG** branch:每個教練一定屬於某個分店，而且每個分店一定有很多個教練
### Relation Schema

## Usage
這個系統主要分兩種操作方式，SQL以及Button
### SQL
* 提供直接輸入SQL指令來操作資料庫

### Button
