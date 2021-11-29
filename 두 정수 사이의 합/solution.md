# 두 정수 사이의 합

```swift
func solution(_ a:Int, _ b:Int) -> Int64 {
    var sum : Int64 = 0
    
    for i in (a<b ? a...b : b...a) {
        sum += Int64(i)
    }
    return sum
}
```   
정수를 더할 변수 `sum`의 초기 값을 0으로 선언   
삼항연산자를 사용해 `a`가 `b`보다 작으면 `a`에서부터 `b`까지,   
`a`가 `b`보다 크면 `b`부터 `a`까지 `sum`에 더한다.