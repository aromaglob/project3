# Project 3 :: AWS EC2 ALB Lab & Investment Analysis

이 저장소는 **AWS 클라우드 인프라(ALB/EC2/ECS)** 실습과 **퀀트 투자 분석 및 알고리즘 트레이딩** 프로젝트를 하나로 묶은 통합 프로젝트 저장소입니다.

---

## 📂 프로젝트 구성

```text
project3/
├── aws-ec2-alb-lab/        # AWS EC2, ALB, ECS, FastAPI, OHLCV 크롤러 실습 환경
├── investment-analysis/    # QuantConnect Lean 백테스트, 기업 가치평가, Qdrant RAG, MongoDB 퀴즈
├── index.html              # 2열 분할 반응형 통합 웹 포털 대시보드
└── README.md               # 프로젝트 안내 문서
```

---

## 🌟 주요 기능 및 디렉토리 안내

### 1. AWS EC2 ALB Lab (`/aws-ec2-alb-lab`)
- **개요**: 클라우드 거버넌스, 온프레미스 vs 클라우드 아키텍처, FinOps 가이드
- **BE-fastapi**: 주식 시세 데이터 제공용 REST API 서버
- **ag-grid-app**: AG Grid 기반의 고성능 금융 시세 그리드 웹앱
- **ohlcv-crawler**: 주식 일봉/분봉 데이터 비동기 크롤러
- **EC2 / ECS / LB**: ALB 타겟 그룹 및 ECS Fargate 배포 스크립트

### 2. Investment Analysis (`/investment-analysis`)
- **개요**: 주식 투자 분석 기초, 기업 가치평가(DCF, RIM, PER/PBR), 자산배분 모델
- **Lean 알고리즘 백테스트**: 현대자동차, 삼성전기 등 주요 종목 알고리즘 트레이딩 전략 성과
- **app**: FastAPI 백엔드 + 순수 JS 프론트엔드 학습 웹앱
- **Qdrant + Ollama RAG**: 벡터 검색 기반 AI 투자 분석 도우미
- **MongoDB**: 금융 및 주식 투자 퀴즈 시스템

---

## 🚀 통합 포털 대시보드 (`index.html`)

저장소 루트에 위치한 `index.html`을 열면 두 프로젝트의 가이드, 아키텍처 다이어그램, 백테스트 요약, 원클릭 터미널 실행 명령어 및 인터랙티브 퀴즈를 하나의 화면에서 편리하게 확인하고 제어할 수 있습니다.

### 실행 방법
브라우저에서 `index.html`을 직접 열거나, 로컬 웹 서버로 실행합니다:
```bash
python -m http.server 8080
# 브라우저에서 http://localhost:8080 접속
```
