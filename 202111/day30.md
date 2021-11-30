### 211130_TIL

------

### 일일회고

------

-  io 공부 위주로 했는데 부족한점이 많은 거같다 처음에 설계를 다 한거?? 같았는데 막상 시작하니

  수정할 부분이 정말 많은거같다

### 오늘 할 것

-  개인프로젝트
-  알고리즘2 문제 풀어보기
-  자바 문법 공부하기

### 오늘 배운것

------

- 개인 프로젝트를 하면서 java io 에대해 공부했다

  개인적으로 내가 만듬 제품들을 어떻게하면 파일에 입/출력 할것인지가 꽤나 많은 고민을 한거 같다

  도중 FileOutputStream 클래스를 통해 내가 미리 지정한 실제파링과 연결을 할 수 있는 기능을 찾아

  BufferedOupputStream  을통해 string 을받아 연결한다

  BufferedOupputStream >  FilterOutputStream  > OutputStream (상속관계)

  https://codehouse.tistory.com/29 , https://sgdev.tistory.com/23 ,자바의정석 15장 을 참고하였다

-   삭제

   삭제하는 메서드를 짤때 에러 사항을 겪었다 입력받은 number 와 실질적으로 productList 가 가지고있는 인덱스의 특정 productnuber 와 일치 시키지 못해 

   ```
    for (int i = 0; i < this.productList.size(); i++) {
         ProductInfo pn = this.productList.get(i);  //인덱스를 하나씩 담아서 비교
   //      System.out.println(pn);
         if (number == pn.getNumber()) {
             this.productList.remove(i);  //
             System.out.println("삭제가 완료 됐습니다");
             break;
         }
     }
   ```

   ProductInfo pn 변수에 인덱스를 하나씩 받아  입력받은 number와 비교해서 삭제
