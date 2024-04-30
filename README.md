Dataset Info.

customers.csv [파일]
고객과 관련된 정보
Customer_id : 고객 ID
Customer_unique_id : 고객 고유 ID
Customer_zipcode_prefix : 고객 우편번호 앞부분
Customer_city : 고객 도시
Customer_state : 고객 주


locations.csv [파일]
지역과 관련된 정보
Geolocation_zipcode_prefix : 우편번호 앞부분
Geolocation_lat : 위도
Geolocation_lng : 경도
Geolocation_city : 도시(city)
Geolocation_state : 주(state)


order_items.csv [파일]
주문 아이템과 관련된 정보
Order_id : 주문 고유 ID
Order_item_id : 동일한 주문에 포함된 품목 수를 식별하는 일련 번호
Product_id : 제품 고유 ID
Seller_id : 판매자 고유 ID
Price : 판매 가격
Freight_value : 품목 화물 가격


orders.csv [파일]
주문과 관련된 정보
Order_id : 주문 고유 ID
Customer_id : 고객 ID
Order_status : 주문 상태
Order_purchase_timestamp : 구매 시간
Order_delivered_carrier_date : 물류 처리 시간
Order_delivered_customer_date : 실제 배송 날짜
Order_estimated_delivery_date : 기대 배송 날짜


payments.csv [파일]
지불과 관련된 정보
Order_id : 주문 고유 ID
Payment_sequential : 결제 시퀀스(둘 이상의 결제 방법으로 결제 가능)
Payment_type : 지불 방법 
Payment_installments : 할부 횟수
Payment_value : 거래 가치


products.csv [파일]
제품과 관련된 정보
Product_id : 제품 고유 ID
Product_category_name : 카테고리 이름
Product_weight_g : 제품 무게(g)
Product_length_cm : 제품 길이(cm)
Product_height_cm : 제품 높이(cm)
Product_width_cm : 제품 너비(cm)


reviews.csv[파일]
Review_id : 리뷰 고유 ID
Order_id : 주문 고유 ID
Review_score : 리뷰 점수
Review_creation_date : 리뷰 생성 시간
Review_answer_timestamp : 리뷰 답변 시간


sellers.csv[파일]
Seller_id : 판매자 고유 ID
Seller_zipcode_prefix : 판매자 우편번호 앞자리
Seller_city : 판매자 도시(city)
Seller_state : 판매자 주(state)
