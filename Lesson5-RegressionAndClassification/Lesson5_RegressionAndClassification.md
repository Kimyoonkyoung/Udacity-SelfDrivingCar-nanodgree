## Regression And Classification

### Difference between Classification And Regression
1. Classification 
* input 이 주어졌을 때, 
    * discrete number of label
    * true/false
    * male/female
    * Binary/Trinary/... Task
* 등으로 ** 분류 ** 를 하는 문제

2. Regression
* input 이 주어졌을 때,
    * 아주 작은 discrete numbur
    * 나이
    * 몸무게
    * Continuous
* 등으로 ** 회귀 ** 를 하는 문제
* '나이' 도 classification 으로 취급하여, 약 150개의 class 로 분류하는 문제로 생각할 수 있지만

  real number 로 표현할 수 있는 분류의 문제는 일반적으로 regression 으로 처리함

3. 결론

Classification vs Regression 은 output 의 종류에 따라 나눌 수 있는 것

Continuous 한 output 이라면, Regression

Discrete 한 output 이라면, Classification


### Classification Learning
1. Instances (=input)
2. Function (=map from input to output)
3. Concept
4. Target Concept (= answer)
5. Hypothesis Class
6. Sample (= training set)
7. Candidate
8. Testing Set