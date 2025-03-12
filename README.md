# Part Inventory System
부품 재고 관리 시스템

### ERD
![erd](https://github.com/user-attachments/assets/644d1714-176d-4594-8347-c3a1987d2c78)


### API 설계
1. 부품(Part) API
|메서드  |엔드포인트         |설명                |
|--------|------------------|--------------------|
|`GET`   |`/parts`          |전체 부품 목록 조회  |
|`GET`   |`/parts/{part_id}`|특정 부품 조회  |
|`POST`  |`/parts`          |새로운 부품 추가     |
|`PUT`   |`/parts/{part_id}`|기존 부품 정보 수정  |
|`DELETE`|`/parts/{part_id}`|특정 부품 삭제       |

2. 부품 입/출고 내역(PartHistory) API
|메서드                |엔드포인트|설명|
|----------------|------------------|-----------------|
|`GET`|`/stock_history`            |전체 입출고 기록 조회    |
|`GET`|`/stock_history/{history_id}` |특정 입출고 기록 조회  |
|`POST`|`/stock_history`|새로운 입출고 기록 추가|

3. 공급업체(Supplier) API
|메서드                |엔드포인트|설명|
|----------------|------------------|-----------------|
|`GET`|`/suppliers`            |전체 공급업체 목록 조회    |
|`GET`|`/suppliers/{supplier_id}` |특정 공급업체 조회  |
|`POST`|`/suppliers`|새로운 공급업체 추가|
