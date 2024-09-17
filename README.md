# 월간 데이콘 - KPI 도출 비즈니스 전략 아이디어 경진대회

## 1. 프로젝트 설명

### 배경
안녕하세요 여러분! 월간 데이콘 - KPI 도출 비즈니스 전략 아이디어 경진대회에 오신 것을 환영합니다.

이 경진대회는 참가자들이 실제 비즈니스 환경에서 발생하는 복잡한 데이터를 분석하고, 기업의 성장과 고객 만족을 도모할 수 있는 전략을 개발하는 능력을 평가합니다. 하지만 제안할 KPI의 최대 수를 3개로 제한하며, 그 이유는 다음과 같습니다:
- 실제 비즈니스 환경에서 모든 데이터를 취합하고 분석하는 것은 불가능할 수 있음을 반영합니다.
- 제한된 데이터 세트를 사용하는 것은 참가자분들이 실제 비즈니스 환경에서 직면할 수 있는 제약 조건을 반영합니다.
  
따라서 참가자들은 제공된 데이터를 통해 가장 영향력 있는 KPI를 식별해야 합니다. 이 경진대회는 데이터 분석과 비즈니스 전략 수립 과정에서 중요한 KPI를 식별하고 정의하는 경험을 제공하는 것을 목적으로 합니다. 이 경진대회에 참가함으로써 데이터 분석 능력을 향상시킬 수 있는 기회를 제공합니다.

### 주제
데이터를 분석하여 핵심 성과 지표(KPI, 예: MAU, CLV 등)를 도출하고, 이를 바탕으로 비즈니스를 위한 전략 방안을 제시하세요.

## 2. 데이터 정보

### **customers.csv [파일]**
고객과 관련된 정보:
- `Customer_id`: 고객 ID
- `Customer_unique_id`: 고객 고유 ID
- `Customer_zipcode_prefix`: 고객 우편번호 앞부분
- `Customer_city`: 고객 도시
- `Customer_state`: 고객 주

### **locations.csv [파일]**
지역과 관련된 정보:
- `Geolocation_zipcode_prefix`: 우편번호 앞부분
- `Geolocation_lat`: 위도
- `Geolocation_lng`: 경도
- `Geolocation_city`: 도시(city)
- `Geolocation_state`: 주(state)

### **order_items.csv [파일]**
주문 아이템과 관련된 정보:
- `Order_id`: 주문 고유 ID
- `Order_item_id`: 동일한 주문에 포함된 품목 수를 식별하는 일련 번호
- `Product_id`: 제품 고유 ID
- `Seller_id`: 판매자 고유 ID
- `Price`: 판매 가격
- `Freight_value`: 품목 화물 가격

### **orders.csv [파일]**
주문과 관련된 정보:
- `Order_id`: 주문 고유 ID
- `Customer_id`: 고객 ID
- `Order_status`: 주문 상태
- `Order_purchase_timestamp`: 구매 시간
- `Order_delivered_carrier_date`: 물류 처리 시간
- `Order_delivered_customer_date`: 실제 배송 날짜
- `Order_estimated_delivery_date`: 기대 배송 날짜

### **payments.csv [파일]**
지불과 관련된 정보:
- `Order_id`: 주문 고유 ID
- `Payment_sequential`: 결제 시퀀스(둘 이상의 결제 방법으로 결제 가능)
- `Payment_type`: 지불 방법
- `Payment_installments`: 할부 횟수
- `Payment_value`: 거래 가치

### **products.csv [파일]**
제품과 관련된 정보:
- `Product_id`: 제품 고유 ID
- `Product_category_name`: 카테고리 이름
- `Product_weight_g`: 제품 무게(g)
- `Product_length_cm`: 제품 길이(cm)
- `Product_height_cm`: 제품 높이(cm)
- `Product_width_cm`: 제품 너비(cm)

### **reviews.csv [파일]**
리뷰와 관련된 정보:
- `Review_id`: 리뷰 고유 ID
- `Order_id`: 주문 고유 ID
- `Review_score`: 리뷰 점수
- `Review_creation_date`: 리뷰 생성 시간
- `Review_answer_timestamp`: 리뷰 답변 시간

### **sellers.csv [파일]**
판매자와 관련된 정보:
- `Seller_id`: 판매자 고유 ID
- `Seller_zipcode_prefix`: 판매자 우편번호 앞자리
- `Seller_city`: 판매자 도시(city)
- `Seller_state`: 판매자 주(state)

## 3. 노트북 설명

### **kpi idea code.ipynb**
이 Jupyter 노트북 파일에서는 주어진 데이터를 불러와 KPI 도출을 위한 데이터 분석을 수행합니다. 주요 내용:
- **데이터 로딩**: `customers`, `locations`, `order_items`, `orders`, `payments`, `products`, `reviews`, `sellers` 등 다양한 데이터셋을 불러오고, 이를 기반으로 KPI를 도출하기 위한 준비를 합니다.
- **KPI 도출**: 고객의 재방문율, 평균 구매 가치(AVG Order Value) 등과 같은 KPI를 정의하고, 이를 기반으로 비즈니스 성장을 위한 전략을 제안합니다.
- **시각화 및 결과 해석**: 데이터 분석 결과를 시각화하고, 도출된 KPI의 비즈니스 의미를 해석하여 실질적인 전략 방안을 제시합니다.
