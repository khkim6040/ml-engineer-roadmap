# Phase 3: 시스템 디자인

> 기간: ~16주 (약 4개월)
> 목표: ML System Design + ML Infra Design 면접 대응 가능

## 디렉토리 구조

```
phase3-system-design/
├── papers/               # 논문 읽기 노트
├── ml-model-design/      # 직접 작성한 ML 시스템 설계
└── ml-infra-design/      # 직접 작성한 ML 인프라 설계
```

## 필수 논문 리스트

| # | 논문 | 핵심 주제 |
|---|------|----------|
| 1 | Deep Neural Networks for YouTube Recommendations | 추천 시스템 기본 구조 |
| 2 | Actions Speak Louder than Words (HSTU) | DLRM vs Generative Rec |
| 3 | Wide & Deep Learning | Feature interaction 기초 |
| 4 | DCN V2 | Explicit cross network |
| 5 | MMoE | Multi-task learning |
| 6 | Yuan Meng - Sequence User Modeling 포스트 | User sequence 처리 |

## 직접 작성할 설계 문서

블로그의 4단계 접근법을 따른다:
1. Problem Framing (clarify → business objectives → ML objectives)
2. High-Level Design (online path + offline path)
3. Step-by-Step Design (retrieval → L1 → L2 → re-ranking)
4. Deep Dives (scaling, cold start, positional bias 등)

### ML Model Design
- [ ] Short Video Recommendations
- [ ] Ads CTR/CVR Ranking
- [ ] 택 1: Search / Trust & Safety / Friend Rec

### ML Infra Design
- [ ] Feature Store
- [ ] Distributed Training Pipeline

## 백엔드 개발자 강점 활용 포인트

- 분산 시스템 (sharding, replication, load balancing) → 이미 알고 있는 내용
- Kafka, Redis, gRPC → 실무 경험 활용
- Feature store = 결국 KV store + streaming pipeline
- Online serving = API 서버 + 캐싱 + 배치 처리
