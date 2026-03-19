# 선형대수 노트

## 3Blue1Brown - Essence of Linear Algebra

### Ep 1. Vectors
#### 벡터란
벡터는 방향과 크기를 표현하는 방법이다.

벡터는 일반적으로 원점을 출발지점으로 생각한다. 따라서 좌표 상의 어떤 점을 벡터로 생각할 수도 있는 것이다.

벡터는 점(point)과 행렬로 표현할 수 있다. 점을 이용해 표현할 때 벡터는 화살표`->`가 되는데 이는 공간을 그래픽으로 표현해서 한눈에 살펴보기 좋고, 행렬로 표현하면 수식으로 만들거나 연산으로 이용하기 좋다.

<img width="365" height="272" alt="image" src="https://github.com/user-attachments/assets/0d7a2f8c-ecde-4a2d-9908-cfe250185d8b" />

개별 벡터는 화살표`->`로, 벡터가 나타낼 수 있는 모든 지점을 생각(span)할 때는 점(선, 면..)으로 생각한다고 한다(Ep 2 내용).

#### 벡터의 합
벡터에 적용되는 기초 연산은 벡터끼리의 합과 벡터의 상수배다.

벡터는 방향과 크기를 포함한다고 했다. 따라서 벡터끼리 더할 때는 각 벡터가 향하는 방향과 그 크기를 더해주면 된다. 간단하게는 한 벡터의 출발지점을 다른 벡터의 끝 지점으로 옮겼을 때 옮겨진 벡터의 종료 지점이 결과 값이 된다.

<img width="334" height="189" alt="image" src="https://github.com/user-attachments/assets/51305ca1-3e8f-4be5-8adc-a57c4773acfa" />

#### 벡터의 상수배
상수배를 통해 벡터의 크기를 키우거나 줄이거나, 반대로 바꿀 수도 있다.

이를 scaling 이라고 한다. 이 때 곱해지는 상수를 scalar라고 한다.

_발음이 `스케일러` 였는데 난 이때까지 `스칼라`로 알고 있었다.. 영어권과 한국어권 발음이 달랐다._

### Ep 2. Linear combinations, span, and basis vectors

#### Basis Vectors
좌표계에서는 어떤 벡터들을 기준으로 다른 모든 벡터를 표현한다. 이때 기준이 되는 벡터들을 **기저벡터(basis vectors)** 라고 한다. 예를 들어 2차원 공간에서는 두 개의 기저벡터를 선택해서, 이 둘의 선형결합(상수배 후 더하기)으로 2차원 공간의 모든 벡터를 표현할 수 있다.

단순하게 생각해서 2차원 공간에서 `[1, 0]`과 `[0, 1]` 두 벡터 쌍은 기저벡터가 될 수 있지만, `[1, 0]`과 `[2, 0]` 은 기저가 될 수 없다. 후자의 경우 아무리 서로 상수배 한 벡터들을 더해봐도 `[x, 0]` 꼴의 벡터들만 표현할 수 있어서 전체 2차원 공간을 만들지 못하기 때문이다.

추가로, 특별한 두 벡터인 `[1, 0]`와 `[0, 1]` 벡터는 각각 î, ĵ 벡터로 부른다.

#### Linear Combinations
위에서 언급한 상수배 한 벡터 두 개를 더하는 것을 **linear combination**이라 한다.

<img width="392" height="206" alt="image" src="https://github.com/user-attachments/assets/522f7160-ef56-4510-840b-6dd5629d6a30" />

Q. 왜 **선형(linear)** 이냐?
A. 스칼라 하나만 변경(아래 사진의 경우 벡터 v의 스칼라 값만 변경)하면서 나오는 지점들을 이어보면 선(line)이 나오기 때문

<img width="396" height="406" alt="image" src="https://github.com/user-attachments/assets/10c0e8db-9d0a-49fd-afa2-ae4d0b0e194f" />

#### Span
이름에서 유추해 볼 수 있듯 확장이란 이름을 가진 span은 주어진 벡터들로 나타낼 수 있는 공간을 나타낸다. 

즉, 두 벡터 v, w의 span은 두 벡터의 linear combination의 집합이다.

<img width="462" height="263" alt="image" src="https://github.com/user-attachments/assets/b888e660-65f6-44f9-84fc-40aca5aae22e" />


벡터가 하나 추가되어도 똑같다. 식에 세 번째 벡터와 그 상수배만 추가된다. 

이 때 생각해보면 좋을 부분은 세 번째 벡터가 앞선 두 개 벡터가 만들어놓은 span을 이동시킨다는 것이다.

앞선 두 개 벡터가 방향이 서로 달랐다면 3차원 공간에서는 아래와 같이 하나의 평면을 span 할 것이다.

<img width="508" height="438" alt="image" src="https://github.com/user-attachments/assets/c33869a9-d1e9-45a0-ab09-c8d1b60abdce" />

세 번째 벡터가 앞선 두 개의 벡터와 방향이 다르다면, 세 번째 벡터가 상수배 되면서 이 평면을 위아래로 움직이게 된다. 이로써 3차원 공간을 span 할 수 있게된다.

<img width="368" height="200" alt="image" src="https://github.com/user-attachments/assets/10e82984-5d31-41c5-b332-44bfb6b8e095" />

<img width="368" height="200" alt="image" src="https://github.com/user-attachments/assets/2a930e46-1f37-497c-8ea0-4e08905d6e74" />

만약 세 번째 벡터가 앞서 span 된 평면 위에 존재한다면, 즉 그 평면과 평행하다면 세 벡터의 span은 3차원이 아니라 여전히 그 평면이 된다. 세 번째 벡터에 어떤 상수배를 하더라도 평면을 위아래로 움직이게 할 수 없기 때문이다. 

<img width="534" height="348" alt="image" src="https://github.com/user-attachments/assets/418df6c2-c49a-46e9-8ea3-41c1c9323cb6" />

#### Linearly Independent
세 번째 벡터가 이미 앞선 두 개의 벡터로 만들어진 span에 놓여진 이 상황의 원인을 생각해보자. 

세 번째 벡터 u를 앞선 두 개 벡터 v와 w로 표현할 수 있기 때문이다. 

이렇게 한 벡터 u를 다른 벡터(v, w)들의 linear combination 으로 표현할 수 있으면 u는 v, w에 **linearly dependent**라고 한다. 만약 표현할 수 없다면 **linearly independent** 라고 한다.

<img width="368" height="201" alt="image" src="https://github.com/user-attachments/assets/0eedf902-0b91-47f3-9ef6-4fa95103e354" />

<img width="361" height="200" alt="image" src="https://github.com/user-attachments/assets/f5531ae8-3bb4-410b-ab76-58531dd17d38" />

#### 문제
Q. 왜 아래 basis 에 대한 정의가 말이 될까?

<img width="600" height="200" alt="image" src="https://github.com/user-attachments/assets/237ae475-3b78-4d88-8ec3-78f49725b275" />

A. 만약 basis of a vector space 가 linearly independent 하지 않다면, 한 벡터는 다른 벡터들의 합으로 치환될 수 있다. 이는 우리가 앞서 봤듯 표현할 수 있는 벡터 공간의 차원을 하나 줄어들게 만든다(3차원 -> 2차원). 따라서 정의에 따라 이런 basis set은 full space를 span하지 못하므로 정의에 모순된다. 

따라서 basis set 안에 있는 벡터들은 서로 linearly independent 해야한다.

---

## Mike X Cohen - Linear Algebra: Theory, Intuition, Code

### 벡터 연산
(학습 후 작성)

### 행렬 곱셈
(학습 후 작성)

### 역행렬
(학습 후 작성)

### 고윳값/고유벡터
(학습 후 작성)

### SVD
(학습 후 작성)
