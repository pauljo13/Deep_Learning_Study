# Deep_Learing_Stuby

## Day 1
### 퍼셉트론 Perceptron
#### 퍼셉트론이란?
퍼셉트론은 프랭크 로젠블라트에 의해 발명된 인공신경망의 초기 형태로, 입력 \(x\)에 가중치 \(w\)를 곱하고 편향 \(b\)를 더하여 그 합이 0을 초과하면 1을 출력하고, 그렇지 않으면 0을 출력합니다. 이는 수학적으로 다음과 같이 표현됩니다:

\[ y = \begin{cases} 
0 & \text{if } \sum_{i} (x_i w_i) + b \leq 0 \\
1 & \text{if } \sum_{i} (x_i w_i) + b > 0 
\end{cases} \]

#### AND, NAND, OR 논리회로
퍼셉트론을 이용하면 AND, NAND, 그리고 OR 등의 기본 논리 회로를 구현할 수 있습니다.

- **AND 게이트**
  | \(x_1\) | \(x_2\) | 출력 |
  |---------|---------|------|
  | 0       | 0       | 0    |
  | 0       | 1       | 0    |
  | 1       | 0       | 0    |
  | 1       | 1       | 1    |

- **NAND 게이트**
  | \(x_1\) | \(x_2\) | 출력 |
  |---------|---------|------|
  | 0       | 0       | 1    |
  | 0       | 1       | 1    |
  | 1       | 0       | 1    |
  | 1       | 1       | 0    |

- **OR 게이트**
  | \(x_1\) | \(x_2\) | 출력 |
  |---------|---------|------|
  | 0       | 0       | 0    |
  | 0       | 1       | 1    |
  | 1       | 0       | 1    |
  | 1       | 1       | 1    |

#### 가중치와 편향 도입
퍼셉트론에서 가중치 \(w\)는 각 입력 신호가 결과에 미치는 영향력을 조절하고, 편향 \(b\)는 출력이 활성화되기 쉬운 정도를 조절합니다.

#### 퍼셉트론의 한계
퍼셉트론은 XOR 문제와 같이 선형적으로 구분되지 않는 경우를 해결하지 못하는 한계를 지닙니다.
**XOR 게이트**
  | \(x_1\) | \(x_2\) | 출력 |
  |---------|---------|------|
  | 0       | 0       | 0    |
  | 0       | 1       | 1    |
  | 1       | 0       | 1    |
  | 1       | 1       | 0    |

#### 다중 퍼셉트론
다중 퍼셉트론은 여러 층의 퍼셉트론을 쌓아 더 복잡한 문제를 해결할 수 있게 해줍니다. 각 층은 여러 뉴런으로 구성되며, 비선형 활성화 함수를 사용하여 비선형 문제도 해결할 수 있습니다.
