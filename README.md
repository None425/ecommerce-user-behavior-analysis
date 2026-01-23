# E-커머스 로그를 활용한 분석

## 프로젝트 개요
E-Commerce 사용자 행동 로그 데이터를 활용하여
사용자의 구매 전환 행동 패턴을 분석하고, 
구매 전환 퍼널 구조를 정의하여 전환율 개선을 위한 
데이터 기반 인사이트 도출을 목표로 한 분석 프로젝트

## 활용 데이터 
1. E-커머스 로그 데이터 - https://www.kaggle.com/code/annettecatherinepaul/ecommerce-analysis-and-recommendations/input
- 주요 변수:
    - event_time
    - event_type (view, cart, purchase)
    - product_id
    - category_code
    - brand
    - price
    - user_id
    - user_session

## 분석 과정
1. 데이터 구조 및 품질 확인
- 데이터 구조(shape, column, dtype) 확인
- 결측치 및 이상치 확인
- 이벤트 타입 분포 확인
- 사용자 및 세션 구조 파악

2. 데이터 전처리
- 결측 데이터 처리
- 카테고리 코드 정리
- 세션 기반 구조 정리

3. 분석 내용
- 구매 전환 퍼널 구조 정의
- view → cart → purchase
- 단계별 전환율 및 이탈률 분석
- 사용자 행동 흐름 분석
- 카테고리별 구매 전환 구조 분석
- 고전환 / 저전환 카테고리 식별
## 분석 결과 및 한계
### 분석 결과
- 전체 사용자 대비 구매 전환율이 낮은 구조로 확인됨
- view → cart 구간에서 가장 큰 이탈 발생
- cart → purchase 구간 또한 주요 병목 구간으로 확인
- 카테고리별 구매 전환 구조 편차가 크게 존재
- 일부 고전환 카테고리가 전체 구매 전환을 견인하는 구조 확인
### 분석의 한계
- 단일 데이터셋 기반 분석으로 다양한 플랫폼 비교 분석에는 한계가 있음

## 활용 기술
- Python : 데이터 분석 및 전처리
- pandas,numpy : 데이터 처리
- Matplotlib : 데이터 시각화
- Jupyter Notebook

## 실행 방법 (데이터셋이 너무 커서 불가)
1. 라이브러리 설치
```bash
pip install -r requirements.txt
```
* Windows 환경에서 pip 오류가 발생할 경우, 아래 명령어 실행 후 다시 실행
```bash
python -m pip install --upgrade pip
```

2. 분석 실행
.ipynb 파일을 Jupyter Notebook에서 실행