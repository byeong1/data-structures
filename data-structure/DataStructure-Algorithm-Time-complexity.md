# 자료구조, 알고리즘의 시간복잡도

A = [ _, _, _, _, _ ] , n : inputSize

1. 모든 입력에 대해 기본 연산 횟수를 더한 후 평균 ( 현실적으로 불가능 )
2. 가장 안좋은 입력(worstacase input)에 대한 기본 연산 횟수를 측정 : worstcase time complexity

- 어떤 입력에 대해서도 W.T.C 보다 수행 시간이 크지 않다!

```
알고리즘 수행시간 = **최악의 입력**에 대한 기본연산 횟수
```

</br>

_예시_

```
algorithm ArrayMax(A, n):
  input : n개의 정수를 갖는 배열 A
  output : A의 수 중에서 최대값 리턴

  currentMax = A[0] <- 1회

  for i = 1 to n-1 do     <- (n-1) x 2 = 2n-2
    if currentMax < A[i]: <- 1회
      currentMax = A[i]   <- 1회 (if currentMax < A[i] 성립 하는 경우 같이 수행)

  return currentMax
```

- currentMax = A[0] : 1
- for 문 : 2n-2

- 2n - 2 + 1 = 2n - 1

```
algorithm ArrayMax의 시간 복잡도 = T

T(n) = 2n-1
```
