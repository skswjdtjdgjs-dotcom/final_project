## [브라질 이커머스 플랫폼 Olist Growth Team 셀러 관리 시스템 구축 프로젝트]
----
### 📌프로젝트 소개
- **데이터셋**: Kaggle Olist 데이터셋 (https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce/data)
- **프로젝트 목표**:
  - Olist 내부 카테고리 전략, 성과 관리, 리스크 관리 담당하는 Growth Team 가정  
  → 셀러 및 플랫폼 안정적 성장 도모
- **프로젝트 기간**: 2025.11 ~ 2025.12
- **사용 프로그램/협업 툴**:
  - 사용 프로그램: Python Vscode, Excel, Tableau
  - 협업 툴: Google Spreadsheet, Notion, Slack, Google Drive
- **멤버 구성**:
  - 정OO(본인): 리스크 파트 분석 및 코드 취합
  - 조OO: 카테고리 파트 분석
  - 안OO: 리스크 파트 분석
  - 이OO: ppt 총괄제작 및 성과 파트 분석
  - 황OO: tableau 대시보드 총괄제작 및 성과 파트 분석
- **기대효과 및 활용방안**:
  - 각 파트별 전략/가이드라인 제시  
   → Growth Team이 공유하는 통합 대시보드 구축  
   → 실시간 분석 및 모니터링에 활용
- **프로젝트 진행**:
  1. 데이터셋 전처리 및 통합
  2. 카테고리 파트 EDA, 분석 및 전략 도출 (동시진행)
  3. 성과 파트 EDA, 분석 및 전략 도출 (동시진행)
  4. 리스트 파트 EDA, 분석 및 전략 도출 (동시진행)
  5. Tableau로 대시보드 구축
  6. PPT 작성

---
### 🔗코드 구성
- **최종 전처리 파일**
  - 각 데이터셋 전처리: 이상치 제거, 표준화, 파생변수 생성
  - 마스터테이블 생성: `Orders`, `Order_items`, `Sellers` 중심 통합
  - 셀러 규모별 Segmentation: 매출 퍼센타일 기준 상위 5% 기준 Enterprise, SMB 구분
- **카테고리 파트 EDA 및 분석**
  - 핵심질문: "카테고리별 특성이 다른데, 동일한 셀러 영입 전략이 효과적일까?"
  - EDA
  - 시장 경쟁도 매트릭스 생성
- **성과 파트 EDA 및 분석**
  - 핵심질문: "셀러 격차는 어떤 운영 및 상품구조에서 발생하는가?"
  - EDA
  - K-means Clustering (k=3)
- **리스크 파트 EDA 및 분석**
  - 핵심질문: "리스크가 있는 셀러를 어떻게 탐지할 수 있을까?"
  - 리스크 지표: 부정 리뷰 비율
  - EDA
  - 리스크 셀러 탐지: 이동평균(window size = 10)
  - 리스크 현황 파악: 감정분석(BERT model) 및 토픽모델링(BERTopic)

---

### ✨최종결과물
- 1️⃣**PPT**: https://drive.google.com/file/d/16ErhpaELD8YjXf34vpGCqjwgzp5GTlbh/view?usp=drive_link
- 2️⃣**Tableau 대시보드**: https://public.tableau.com/app/profile/seongheon.jeong/viz/TeamSonoOlistAnalysisDashboard/_overview
  - Overview
  - Catergory
  - Seller
  - Risk








