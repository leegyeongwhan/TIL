### 211201_TIL

------

### 일일회고

------

-  gui 에서 구현한 변화된 수량을 파일 io로 받고싶었는데 나중에 더 생각해봐야겠다

### 오늘 할 것

-  개인프로젝트 자판기 만들기

### 오늘 배운것

------

-  사용자쪽으로 가면 gui를 이용해 번튼을 누르면 그에 따라 반응하도록 구현해보았다

- gui를 구현하다 저번주부터 awt swig 버튼 에서 막히는 부분이있다

  - ```
    if (jb1.isSelected()) {
        name = finalList.get(0).getName();
        price = finalList.get(0).getPrice();
    } else if (jb2.isSelected()) {
        name = jb2.getName();
        price = finalList.get(1).getPrice();
    } else if (jb3.isSelected()) {
        name = jb3.getName();
        price = finalList.get(2).getPrice();
    } else if (jb4.isSelected()) {
        name = jb4.getName();
        price = finalList.get(3).getPrice();
    }
    ```

이런식으로 버튼을 눌렀을떄 인덱스에 맞는 값을 주고싶은데 하드코딩하게 된다 더 좋은방법이

있을거같은데 찾지 못했다..

