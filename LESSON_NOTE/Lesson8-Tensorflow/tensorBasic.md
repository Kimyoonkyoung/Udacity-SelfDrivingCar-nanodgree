tf.constant 는 상수임
tf.constant('string')
tf.constant(1234)
tf.constant([123,123,123])
tf.constant([123,123],[234,234])

Session
operation을 할당시켜서 실행하게끔 하는것

PlaceHolder (변수개념)
placeholder 는 tensor를 리턴해준다
그래서, tf.session.run 할때 값을 넣을 수 있게도와준다

feed_dict
여러개의 tensor 에 값을 할당해줄 수 있게 해줌

Math
tf.add(5,2) = 7
tf.subtract(10,4) = 6
tf.multiply(2,5) = 10

cast
tf.cast(x, tf.int32)
 ex) tf.subtract(tf.cast(tf.constant(2.0), tf.int32), tf.constant(1)) = 1
 
tf.Variable 
변수를 저장할 수 있음
x = tf.Variable(5)
session 에 들어가기 전에 tf.global_variables_initializer() 를 써줘야함

tf.truncated_normal()
정규분포의 랜덤수를 추출함
n_features = 120, n_labels = 5,
weight = tf.Variable(tf.truncated_normal((n_features, n_labels)))

tf.zeros()
전부 다 0으로 셋팅
n_labels = 5
bias = tf.Variable(tf.zeros(n_labels))

tf.nn.softmax([2.0, 1.0, 0.2])
소프트맥스

tf.reduce_sum()
배열을넣으면 그 요소들을 다 더한다
tf.reduce_sum([1,2,3,4,5]) = 15

tf.log(100)
말그대로 로그

tf.relu 
relu

변수나 모델 저장하기
saver 사용
tf.train.Saver.save(sess, file명) 함수
저장 파일은 *.ckpt (checkpoint)

저장된거 불러오기
tf.train.Saver.restore(sess, file명)
save 할때있었던 변수들을 다시 선언해두어야 한다

dropout
tf.nn.dropout(노드수, 남길노드수)
1/남길노드
보통 트레이닝 할때는 0.5로시작
테스팅에는 1




