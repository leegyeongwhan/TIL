### 2111117_TIL

------

### 일일회고
------

- 어제 오늘 몸이 안좋아 코딩과 학습을 많이하지 못했다.. 항상 컨디션관리에 유념하자  공부 학습도 좋지만 건강이 최우선이다


### 오늘 할 것

- 한글시계 추가 미션수행하기
- 자기전 java 문법 두시간공부

### 오늘 배운것

------

- 같이 공부하는 조원들로부터  enum 클래스에 대해 알게됐다

  - JAVA에서 열거 상수는 상수 각각을 내부적으로 public static final 필드이면서 객체로 제공되도록 한다 jvm 메서드영억에서 상주 시켜 프로그램이 종료되기 진적까지 언제든지 쓸수있다

  - switch 타입은 사용자 타입을 못쓴다

  - enum은 그동안의 자바문법과는 다르다 열거형이라 부르고 열거형은 서로 연관된 상수들의 집합이다

  - ```
    class Fruit {
        public static final Fruit APPLE = new Fruit();
        public static final Fruit PEACH = new Fruit();
        public static final Fruit BANANA = new Fruit();
    
    }
    enum Fruit{
        Apple,Peach,Banan
    }
    ```

    ​	두개는 같다

  - 필드와 메서드를 온전히 가질수있는 

- 날짜,시간을 구하는 java의 LocalDateTime 클래스

