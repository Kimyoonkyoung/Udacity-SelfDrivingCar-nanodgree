## NeuralNet

1. 퍼셉트론
퍼셉트론은 인풋*웨잇트를 썸하고
단순한 세타를 기준으로 0/1 의 아웃풋만 내는 아주 단순한 뉴런 구조를 말한다
linear 하게 나눌 수 있는 문제에서 적용가능  (and, or, not)

2. 퍼셉트론 트레이닝
input 에서 output으로 가게 해주는 weight 를 찾는 것 
- perceptron rule : threshold 존재
- gradient descent/delta rule : threshold 없

- learning rate : 이동 방향으로의 양 

3. Gradient descent
non-linear separate 문제에서 활용
(1/2 하는거 이해 못함)

4. optimizing weights
- momentum
- higher order derivatives
- randomized optimization
- penalty for "complexity"

로컬미니멈에 빠지지 않기 위해서 초기 웨이트를 랜덤으로 뽑는다
낮은 복잡도로 시작하기 위해서 초기 웨이트를 작은 값으로 설정한다

퍼셉트론 - th유닛
perceptron rule
general