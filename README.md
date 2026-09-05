# Smart-SPC

### ML-Assisted Semiconductor Process Monitoring and Sensor Diagnosis

반도체 공정 데이터를 기반으로 **SPC를 통한 공정 이상(OOC) 탐지**와  
**XGBoost + SHAP을 활용한 주요 센서 분석**을 수행하는 공정 모니터링 프로젝트입니다.

##  Workflow

```text
Process Data
     ↓
Data Preprocessing
     ↓
EWMA-based SPC
     ↓
OOC Detection
     ↓
XGBoost + SHAP
     ↓
Sensor Priority Ranking
     ↓
Spotfire Dashboard
 Key Features
Automatic Preprocessing — 결측치, Zero Variance, Target 등을 자동 처리
EWMA-based SPC — 공정 데이터의 이상 상태(OOC) 탐지
XGBoost — Pass/Fail 분류 및 불량 관련 Feature 분석
SHAP — 주요 센서의 영향도 및 조사 우선순위 도출
Spotfire — SPC 및 센서 분석 결과 Dashboard 시각화
 Tech Stack

Python · Pandas · NumPy · XGBoost · SHAP · SPC · Spotfire

 Output
Sensor Priority

센서별 OOC 발생량과 ML 기반 Feature Importance를 활용하여
분석 우선순위를 도출합니다.

SPC Time-Series

Raw Value, EWMA, UCL, LCL 및 OOC Signal을 시간 흐름에 따라 시각화합니다.

 Project Concept

SPC → 공정 이상 탐지
XGBoost → 불량 분류
SHAP → 주요 센서 분석
Spotfire → 공정 모니터링

본 프로젝트는 특정 데이터셋에 종속되지 않고 다양한 **구조화된 공정 데이터(CSV 등)**에 적용할 수 있는 분석 파이프라인 구축을 목표로 합니다.
