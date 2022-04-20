# 수박수박수박수박수박수?

```swift
func solution(_ n:Int) -> String {
    let result = String(repeating: "수박", count: n/2) + ((n % 2 == 0) ? "" : "수")
    return result
}
```     

특정 문자열을 반복시켜주는 ` repeat` 함수를 사용한다.   
입력 받은 숫자가 홀수일 경우, `"수"`를 더하여 출력한다.   

[문제](https://programmers.co.kr/learn/courses/30/lessons/12922)