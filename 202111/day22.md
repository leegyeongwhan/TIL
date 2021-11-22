### 211122_TIL

------

### 일일회고

------

- 오늘은 그래도 코딩과 학습을 적절히 균형있게한 것같다 awt swing은 처음보는 문법들이 많아 여러모로 어려운 학습인 거같다 내일도 다시봐보자!


### 오늘 할 것

## 

- gui프로그래밍 학습하기 0
- awt/swing 학습하기 0
- Java 8 람다와 스트림 
- for-each, map, filter 사용법
- 자바의 인터페이스
- 제네릭 사용법

### 오늘 배운것

------

- awt
  - os 리소스를 많이 소모
  - os 에 부담을 줌
  - 실행되는 os마다 외양이 바뀔수가있다
- swing
  - awt기술 기반으로 작성된 라이브러리
  - 운영체제에 도움을 받지 않고 구현 >> 순수 자바 언어로 작성

- api

  - 프로그램을 만들떄 다양한 장치가있다 우리는 이것을 "직접" 상용하는 것이 아닌 인터페이스를 통해 간적접으로 사용하는것 이것을 어플리케이션을 만들떄 사용하는것 >api

    즉 우리는 api 라는 인터페이스를 통해 간접적으로 이용해 어플리케이션을 만든다

- 간단 rpg 게임만들기 구현완료

- 참조변수 this와 super
  - this 는 지역변수,인스턴스 변수 구분, 단 상속관계에서 자손에 맞는 인스턴스 변수가 가 없으면 조상을 가르킴
  - 참조변수 super는 상속관계의 조상 을 가르킨다
  - 둘은 조상과 자신의 맴버를 구분할떄 쓴다
- super()
  - 참조변수 super와비교하자 둘은 상관이없다
  - 생성자super는 조상 생성자를 호출할떄쓴다  > 상속받을때 생성자와 초기화 블럭은 상속이 안되기때문!

```
class Point {
    int x = 0;
    int y = 0;
    Point(int x,int y){
    	this.x=x;
    	this.y=y;
    }
}

public class ex_11 extends Point {
    int z = 0;

    ex_11() {
        super(x,y);
        this.z = 3;
    }

}
```

조상의 맴버는 조상의 생성자를 통해 초기화하자

- 생성자의 첫 줄에는 반드시 다른생성자를 호출해야 한다!!!!

- 추상클래스

  - 추상 메서드를 가지고있는 클래스 추상메서드(구현부가 없는 메서드)

  - 미완성설계도 즉 객체(인스턴스)를 만들 수없다

  - abstract 를붙여줘 자손에서 조상 메서드를 구현해줘야한다

    - 모두 다구현 하지않을때는  구현 하지않은 메서드는  abstract를 붙여줘야한다

  - ```
    abstract class Player {
        abstract void play(int pos);
        abstract void stop();
    }
    class AudioPlayer extends Player {
        void play(int pos) {System.out.println(pos);}
        void stop() {System.out.println("stop");}
    }
    public class ex_11 {
        public static void main(String[] args) {
            Player p  = new AudioPlayer();
            p.play(100);
            p.stop();
        }
    }
    ```

    player 타입의 참조변수 p 로 adioplayer를 가르켜도 이상이없다 player의 인스턴스는 생성이 안돼있지만

    audio는 생성이 되어있어 상관없다!

- 캡슐화

  - 클래스의 맴버 변수를 다룰때 직접 다루지말고 메서드를 통해 다루자 변수는private 메서드는 public ex) getter ,setter ,시계 class 시분초

   

- for each문

  - 자료구조와 배열과 잘 어울리는 반복문 구문인거같다

- 스택 관련 알고리즘
  - pop 과 push에대해 간단하게 배웠다 peek을이용하면 스택에 쌓인 가장 위에 요소를 쓸수있다
