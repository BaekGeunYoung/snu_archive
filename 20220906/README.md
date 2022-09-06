
- an algorithm is any well-defined computational procedure that takes
some value, or set of values, as input and produces some value, or set of values, as
output. An algorithm is thus a sequence of computational steps that transform the
input into the output.

- parallelism은 어려워서 안함

- 35 page - comparison of running times 해보기

### 2-1. insertion sort

2 important this in data structure & algorithm

- correctness
- efficiency

loop invariant
- a statement which can prove the correctness of an algorithm

loop invariant를 이용한 algorithm induction 과정에서 line# of algorithm를 꼭 명시해야 함

loop invariant of insertion sort

- At the start of each iteration of the for loop of lines 1–8, the subarray
A[1 .. j-1] consists of the elements originally in A[1 .. j-1], but in sorted
order.

loop invariant should meet below 3 requirements:

- initialization: loop에 진입하는 시점에 loop invariant가 참이어야 함
- maintenance: 직전 수행에서 loop invariant가 참일 때, 다음 수행도 참이어야 함
- termination: loop가 종료되었을 때 loop invariant가 참이어야 함

loop invariant은 어떻게 얻는가?
- termination condition에서 우리가 원하는 문장을 얻을 수 있도록 loop invariant을 design해야 함!

### 2-2. Analyzing algorithms

correctness induction 과정에서도 line# 가 중요했듯이, time complexity 분석에도 line#가 매우 중요!

time complexity of an algorithm: algorithm의 각 line이 실행된 횟수를 합친 것!

average case time complexity 중요

### 2-3. designing algorithm

2-3-1. divide-and-conquer approach

Divide - Conquer - Combine
