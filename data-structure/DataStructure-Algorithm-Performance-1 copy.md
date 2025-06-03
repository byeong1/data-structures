# 자료구조와 알고리즘 성능 1

- 가상 컴퓨터 (Virtual Machine) + 가상 언어(Pseudo Language) + 가상 코드(Pseudo Code)

</br>

## 1. 가상 컴퓨터

Turing Machine -> von Neumann : RAM (Random Access Machine)  
 RAM = CPU + Memory + **기본 연산**

```
[기본 연산] - 1단위 시간
- 단위 시간에 수행되는 연산
- 배정, 대입, 복사
- 산술 ( +, -, *, / )
- 비교 ( >, >=, <, <=, ==, != )
- 논리 ( AND, OR, NOT )
- 비트 ( bit-AND, OR, NOT )
```

</br>

## 2. 가상 언어

- 배정, 산술, 비교, 논리, bit-논리 : 기본 연산 표현
- 비교 : if, if ... else, if ... elseif ... else
- 반복 : for, while
- 함수 : 정의, 호출, return

</br>

## 3. 가상 코드

```
algorithm ArrayMax(A, n):
  input : n개의 정수를 갖는 배열 A
  output : A의 수 중에서 최대값 리턴

  currentMax = A[0]

  for i = 1 to n-1 do
    if currentMax < A[i]:
      currentMax = A[i]

  return currentMax
```
