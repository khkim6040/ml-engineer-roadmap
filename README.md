# ML Engineer Roadmap

> 백엔드 개발자가 MLE Interview 2.0을 소화하기 위한 로드맵
>
> 원문: [MLE Interview 2.0: Research Engineering and Scary Rounds](https://www.yuan-meng.com/posts/mle_interviews_2.0/) by Yuan Meng

**페이스**: 하루 30분, 주 ~3.5시간  
**총 예상 기간**: ~20개월  
**시작일**: 2026-03-17

---

## 📊 진행 현황

| Phase | 기간 | 시작 | 종료(예상) | 상태 |
|-------|------|------|-----------|------|
| Phase 0: 수학 기초 | ~20주 | 2026-03 | 2026-08 | 🟡 진행중 |
| Phase 1: ML/DL 기초 | ~24주 | 2026-08 | 2027-01 | ⚪ 대기 |
| Phase 2: PyTorch/ML 코딩 | ~20주 | 2027-01 | 2027-06 | ⚪ 대기 |
| Phase 3: 시스템 디자인 | ~16주 | 2027-06 | 2027-10 | ⚪ 대기 |
| Phase 4: 면접 준비 | Phase 2부터 병행 | - | - | ⚪ 대기 |

---

## Phase 0: 수학 기초 (~20주)

> 모든 ML 학습의 전제 조건. 여기를 건너뛰면 Phase 2부터 벽에 부딪힌다.

### 선형대수 (8주)

**주 1-2: 직관 잡기 — 3Blue1Brown**
- [ ] Ep 1. Vectors, what even are they?
- [ ] Ep 2. Linear combinations, span, and basis vectors
- [ ] Ep 3. Linear transformations and matrices
- [ ] Ep 4. Matrix multiplication as composition
- [ ] Ep 5. Three-dimensional linear transformations
- [ ] Ep 6. The determinant
- [ ] Ep 7. Inverse matrices, column space and null space
- [ ] Ep 8. Nonsquare matrices as transformations
- [ ] Ep 9. Dot products and duality
- [ ] Ep 10. Cross products
- [ ] Ep 11. Cross products in the light of linear transformations
- [ ] Ep 12. Cramer's rule
- [ ] Ep 13. Change of basis
- [ ] Ep 14. Eigenvectors and eigenvalues
- [ ] Ep 15. A quick trick for computing eigenvalues
- [ ] Ep 16. Abstract vector spaces

> 🔗 [YouTube 재생목록](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)

**주 3-8: 코드와 함께 — Mike X Cohen "Linear Algebra: Theory, Intuition, Code"**
- [ ] 벡터 연산 (내적, 외적, norm)
- [ ] 행렬 곱셈과 연산
- [ ] 역행렬과 연립방정식
- [ ] 행렬 공간 (column space, null space, rank)
- [ ] 고윳값과 고유벡터
- [ ] 특이값 분해 (SVD)
- [ ] 주성분 분석 (PCA) 기초

### 미적분 (5주)

**주 9-10: 직관 잡기 — 3Blue1Brown "Essence of Calculus"**
- [ ] Ep 1-4: 미분의 본질, 도함수
- [ ] Ep 5-6: chain rule (핵심!)
- [ ] Ep 7-8: 적분 기초
- [ ] Ep 9-12: 테일러 급수 등 나머지

> 🔗 [YouTube 재생목록](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)

**주 11-13: 편미분과 gradient — Khan Academy**
- [ ] Partial derivatives
- [ ] Gradient 개념
- [ ] Chain rule (다변수)
- [ ] Gradient descent 직관 (코드로 직접 구현)

> 🔗 [Khan Academy Multivariable Calculus](https://www.khanacademy.org/math/multivariable-calculus)

### 확률/통계 (5주)

**주 14-16: StatQuest 핵심 영상**
- [ ] Probability vs Likelihood
- [ ] Bayes' Theorem
- [ ] 정규분포 (Normal Distribution)
- [ ] 이항분포, 베르누이
- [ ] 기대값과 분산
- [ ] Maximum Likelihood Estimation (MLE)
- [ ] Cross-entropy와 KL divergence
- [ ] p-value, 가설검정 기초
- [ ] Confusion matrix, ROC, AUC
- [ ] Bias-Variance tradeoff

> 🔗 [StatQuest YouTube](https://www.youtube.com/@statquest)

**주 17-18: Python 시뮬레이션**
- [ ] 동전 던지기로 MLE 구현
- [ ] 중심극한정리 시뮬레이션
- [ ] Naive Bayes 분류기 from scratch

### 체크포인트 (2주)

**주 19-20: 복습 + 셀프 테스트**
- [ ] ✅ "softmax가 왜 확률분포가 되는지" 설명 작성
- [ ] ✅ "gradient descent가 왜 loss를 줄이는지" 설명 작성
- [ ] ✅ "행렬곱이 왜 신경망의 forward pass인지" 설명 작성
- [ ] `phase0-math/checkpoint.md`에 정리 후 커밋

---

## Phase 1: ML 기초 + 딥러닝 (~24주)

### 전통 ML (10주)

**Andrew Ng — Machine Learning Specialization (Coursera)**
- [ ] Course 1: Supervised ML — Week 1 (Linear Regression)
- [ ] Course 1: Supervised ML — Week 2 (Multiple Regression, Gradient Descent)
- [ ] Course 1: Supervised ML — Week 3 (Logistic Regression, Classification)
- [ ] Course 2: Advanced Learning Algorithms — Week 1 (Neural Networks)
- [ ] Course 2: Advanced Learning Algorithms — Week 2 (NN Training)
- [ ] Course 2: Advanced Learning Algorithms — Week 3 (Decision Trees)
- [ ] Course 2: Advanced Learning Algorithms — Week 4 (Ensemble, Random Forest)
- [ ] Course 3: Unsupervised Learning — Week 1 (Clustering, K-Means)
- [ ] Course 3: Unsupervised Learning — Week 2 (Anomaly Detection)
- [ ] Course 3: Unsupervised Learning — Week 3 (Recommender Systems)

> 🔗 [Coursera ML Specialization](https://www.coursera.org/specializations/machine-learning-introduction)

### 딥러닝 기초 (12주)

**"Understanding Deep Learning" — Simon Prince (무료)**
- [ ] Ch 1: Introduction
- [ ] Ch 2: Supervised Learning
- [ ] Ch 3: Shallow Neural Networks
- [ ] Ch 4: Deep Neural Networks
- [ ] Ch 5: Loss Functions
- [ ] Ch 6: Training Models (Gradient Descent, Backprop)
- [ ] Ch 7: Gradients and Initialization
- [ ] Ch 8: Measuring Performance
- [ ] Ch 9: Regularization
- [ ] Ch 11: Residual Networks
- [ ] Ch 12: Transformers

> 🔗 [UDL Book (무료 PDF)](https://udlbook.github.io/udlbook/)
> 🔗 [Colab Notebooks](https://github.com/udlbook/udlbook)

각 챕터마다: 읽기 4일 + 노트북 실습 3일 = 1주/챕터

### 정리 (2주)
- [ ] 각 챕터 핵심 요약 `phase1-ml-basics/understanding-dl/` 에 커밋
- [ ] scikit-learn 기본 사용법 치트시트 정리

---

## Phase 2: PyTorch + ML 코딩 (~20주)

### PyTorch 입문 (3주)

- [ ] Sebastian Raschka "PyTorch in One Hour" 읽기 (3일)
- [ ] TensorGym 매일 1-2문제 (2주, 총 20-30문제)

> 🔗 [PyTorch in One Hour](https://sebastianraschka.com/teaching/pytorch-1h/)
> 🔗 [TensorGym](https://tensorgym.com/)

### Transformer from scratch — Karpathy 시리즈 (10주)

**micrograd: autograd 이해 (주 1-2)**
- [ ] 영상 시청: "The spelled-out intro to neural networks and backpropagation"
- [ ] micrograd 코드 직접 재현
- [ ] `phase2-pytorch/micrograd/` 에 커밋

**makemore: 언어모델 기초 (주 3-5)**
- [ ] Part 1: Bigram model
- [ ] Part 2: MLP
- [ ] Part 3: Activations & Gradients, BatchNorm
- [ ] 각 파트 코드 재현 후 커밋

**nanoGPT: Transformer 직접 구현 (주 6-10)**
- [ ] "Let's build GPT from scratch" 영상 시청 (여러 날에 나눠서)
- [ ] Embedding + Positional Encoding 구현
- [ ] Self-Attention 구현
- [ ] Multi-Head Attention 구현
- [ ] FeedForward (MLP) 구현
- [ ] Transformer Block 구현
- [ ] Decoder 전체 조립
- [ ] Training loop 구현
- [ ] 텍스트 생성 (inference) 구현
- [ ] `phase2-pytorch/nanogpt/` 에 커밋

> 🔗 [Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html)
> 🔗 [nanoGPT repo](https://github.com/karpathy/nanoGPT)

### ML 코딩 연습 (7주)

**Deep-ML (주 11-15)**
- [ ] Easy 5문제+ (KNN, Linear Regression, Sigmoid 등)
- [ ] Medium 5문제+ (Logistic Regression, K-Means, PCA 등)
- [ ] Hard 3문제+ (Attention, Transformer components 등)

> 🔗 [Deep-ML](https://www.deep-ml.com/problems)

**numpy-100 (주 16-17)**
- [ ] 1-25번
- [ ] 26-50번
- [ ] 51-75번
- [ ] 76-100번

> 🔗 [numpy-100 repo](https://github.com/rougier/numpy-100)

---

## Phase 3: 시스템 디자인 (~16주)

> 백엔드 개발자 배경이 여기서 가속기가 된다.

### ML System Design (10주)

**논문 읽기 (주 1-6)**
- [ ] YouTube 추천 논문: "Deep Neural Networks for YouTube Recommendations"
- [ ] HSTU: "Actions Speak Louder than Words"
- [ ] Deep & Wide: "Wide & Deep Learning for Recommender Systems"
- [ ] DCNv2: "DCN V2: Improved Deep & Cross Network"
- [ ] MMoE: "Modeling Task Relationships in Multi-task Learning"
- [ ] Sequence Modeling 관련 자료 (Yuan Meng 블로그 포스트)

**직접 설계 작성 (주 7-10)**
- [ ] Short Video Recommendations 설계
- [ ] Ads CTR/CVR Ranking 설계
- [ ] 택 1: Search / Trust & Safety / Friend Recommendations

> 각 설계를 `phase3-system-design/ml-model-design/` 에 마크다운으로 커밋

### ML Infra Design (6주)

**학습 (주 11-14)**
- [ ] Yuan Meng ML Infra 포스트 정독
- [ ] "Distributed Machine Learning Patterns" 핵심 챕터
- [ ] NeetCode System Design — ML 관련 파트만
- [ ] Hello Interview "System Design in a Hurry"

**직접 설계 작성 (주 15-16)**
- [ ] Feature Store 설계
- [ ] Distributed Training Pipeline 설계

---

## Phase 4: 면접 준비 (Phase 2부터 병행)

### LeetCode (Phase 2 시작 시점부터 지속)

> NeetCode 250 기준, 주 2-3문제. LC 하는 날 / ML 하는 날 교대.

**Arrays & Hashing**
- [ ] 5문제+

**Two Pointers / Sliding Window**
- [ ] 5문제+

**Stack / Queue**
- [ ] 5문제+

**Binary Search**
- [ ] 5문제+

**Trees / Graphs**
- [ ] 10문제+

**Dynamic Programming**
- [ ] 10문제+

**기타 (Heap, Greedy, Backtracking, etc.)**
- [ ] 10문제+

> 🔗 [NeetCode 250](https://neetcode.io/practice)

### OOP 코딩 (Phase 3 시점, 2-3주 집중)

- [ ] Coditioning OOP crash course 수강
- [ ] NeetCode Design Patterns 수강
- [ ] KV Store 구현
- [ ] Rate Limiter 구현
- [ ] LRU Cache 구현

> 🔗 [Coditioning](https://www.coditioning.com/app/learning/courses/tech_interview_prep/4)
> 🔗 [NeetCode Design Patterns](https://neetcode.io/courses/design-patterns/10)

### Behavior (면접 직전 2주)

- [ ] 79개 질문 중 시그널별 대표 15개 선정
- [ ] 각 질문마다 SAIL 스토리 작성
- [ ] 회사별 values에 맞춰 스토리 조정

---

## 📚 핵심 리소스 모음

| 카테고리 | 리소스 | 유형 |
|----------|--------|------|
| 선형대수 | 3Blue1Brown "Essence of Linear Algebra" | 영상 |
| 선형대수 | Mike X Cohen "Linear Algebra: Theory, Intuition, Code" | 책 |
| 미적분 | 3Blue1Brown "Essence of Calculus" | 영상 |
| 확률/통계 | StatQuest | 영상 |
| 전통 ML | Andrew Ng ML Specialization (Coursera) | 코스 |
| 딥러닝 | "Understanding Deep Learning" — Simon Prince | 책 (무료) |
| PyTorch | Sebastian Raschka "PyTorch in One Hour" | 문서 |
| PyTorch 연습 | TensorGym | 사이트 |
| Transformer | Karpathy "Neural Networks: Zero to Hero" | 영상 |
| ML 코딩 | Deep-ML | 사이트 |
| NumPy | numpy-100 | repo |
| ML 시스템 디자인 | Yuan Meng 블로그 시리즈 | 블로그 |
| ML Infra | "Distributed Machine Learning Patterns" | 책 |
| 시스템 디자인 | NeetCode System Design | 코스 |
| 시스템 디자인 | Hello Interview | 사이트 |
| LC | NeetCode 250 | 사이트 |
| OOP | Coditioning OOP crash course | 코스 |
| LLM 구현 | "Build a Large Language Model from Scratch" | 책 |

---

## 🏷️ 커밋 컨벤션

```
[phase] 간단한 설명

예시:
[phase0] 선형대수 - 고윳값/고유벡터 노트 정리
[phase1] UDL Ch5 Loss Functions 노트북 실습
[phase2] micrograd Value 클래스 구현
[phase3] YouTube 추천 논문 읽기 노트
[phase4] LC #200 Number of Islands 풀이
```

---

## 📝 학습 원칙

1. **하루 30분, 매일** — 양보다 일관성
2. **Action first** — 이론을 다 이해하고 코드 치는 게 아니라, 코드 치면서 이론을 이해한다
3. **커밋 = 학습 기록** — 불완전해도 매일 커밋
4. **체크포인트** — 각 Phase 끝에서 자기 말로 설명할 수 있는지 확인
