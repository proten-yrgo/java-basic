# 📌 문제 이름

> [PCCE 기출문제] 1번 / 문자 출력

## 🔗 문제 링크

- [문제 바로가기](https://school.programmers.co.kr/learn/courses/30/lessons/340207)

## 💡 문제 해결 전략

3
2
1
Let's go!

처음 봤을 땐 줄바꿈이 가장 눈에 들어왔습니다. 그리고 주어진 코드를 봤을 때 string message = "(빈칸)"; 을 보고 해당 빈칸에 Let's go! 입력해야 된다고 판단, 
 cout << "3(빈칸)2(빈칸)1" << endl;
    cout << message << endl;
을 보고 "3(빈칸)2(빈칸)1" 을 줄바꿈 하려면 /n을 써야겠다고 생각하였습니다.

## 💻 코드

```java
#include <iostream>

using namespace std;

int main(void) {
    string message = "
Let's go!
";

    cout << "3
\n
2
\n
1" << endl;
    cout << message << endl;

    return 0;
}
```

## 📝 비고

<!-- 풀면서 겪은 어려운 점, 주의해야 할 점, 못 풀었다면 왜 못 풀었는지 등 생각나는 것을 자유롭게 적어주세요. 없으면 생략 가능합니다 -->
<!-- ⚠️ 답을 봤다면 반드시 "답을 봤다"고 적어주세요! (복습 및 자가 점검용) -->

- [O] 스스로 해결
- [ ] 답을 보고 해결
- [ ] 못 풀었음
