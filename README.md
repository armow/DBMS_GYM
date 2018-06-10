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
