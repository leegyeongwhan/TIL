### 211209_TIL

------

### 일일회고

------

-  마스터즈 코스 코딩 테스트 보고 멘탈이 탈탈털렸다..

### 오늘 할 것

-  알고리즘

### 오늘 배운것

------

- ```
  public int[] solution(int[] array, int[][] commands) {
    int[] answer = new int[commands.length];
    int[] str;
    int a = 0;
    for (int i = 0; i < commands.length; i++) {
      str = Arrays.copyOfRange(array, commands[i][0] - 1, commands[i][1]);
      Arrays.sort(str);
      a = str[commands[i][2] - 1];
      answer[i] = a;
    }
    return answer;
  ```

copyOfRange,와 sort를 활용해 보았다
