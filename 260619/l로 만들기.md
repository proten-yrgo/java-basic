# 📌 문제 이름

> 예: l로 만들기

## 🔗 문제 링크

- [문제 바로가기](https://school.programmers.co.kr/learn/courses/30/lessons/181834)

## 💡 문제 해결 전략

먼저 주어진 문자열을 배열로 다루고 싶어서 처음엔 List로 할까 생각하다가 List가 생각이 안 나서
문자열을 배열로 담는 방법을 검색하였고 char[] arr = myString.toCharArray(); 가 생각했던 작동과 동일하여 사용함.
이후 for문은 직접 작성. myString을 배열에 담아 문자열의 길이만큼 확인하는데, 아스키 값으로 비교될 거라 생각하여
l보다 작은 문자를 l로 대체하게끔 하였습니다.

## 💻 코드

```java
class Solution {
    public String solution(String myString) {
        
        char[] arr = myString.toCharArray();
        
        for (int i = 0; i < myString.length(); i++) {
            if (arr[i] < 'l') {
                arr[i] = 'l';
            }
        }

        return new String(arr);
    }
}
```

## 📝 비고

<!-- 풀면서 겪은 어려운 점, 주의해야 할 점, 못 풀었다면 왜 못 풀었는지 등 생각나는 것을 자유롭게 적어주세요. 없으면 생략 가능합니다 -->
<!-- ⚠️ 답을 봤다면 반드시 "답을 봤다"고 적어주세요! (복습 및 자가 점검용) -->

문자열을 배열로 담고는 싶은데 어떤 걸 사용해야할지 또는 사용방법을 잘 몰라서 거기가 막혔음.
char[] arr = myString.toCharArray();에 대해 검색하면서 
char ch = myString.charAt(0); 인덱스로 접근하는 방법 및
public String solution(String myString) {

    List<Character> list = new ArrayList<>();

    for (char c : myString.toCharArray()) {
        list.add(c);
    }

    System.out.println(list.get(0));

    return myString;
}
처음 생각했던 리스트 방식도 알게 되었습니다.

- [x] 스스로 해결
- [ ] 답을 보고 해결
- [ ] 못 풀었음
