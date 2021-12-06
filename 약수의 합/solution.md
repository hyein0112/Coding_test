# 약수의 합

```swift
func solution(_ n:Int) -> Int {
    var sum = 0
    if n == 0 {return 0}
    
    for i in 1...n {
        if n%i==0 {
            sum += i
        }
    }
    return sum
}
```

`n`의 약수의 합을 받는 변수 `sum`의 초기 값을 0으로 선언  
`if`문을 사용해 `n`이 0일 때 0을 반환한다.   
`for`문을 사용해 1부터 `n`까지 범위를 준 뒤 `if`문으로 `n`의 약수를 더한다.   


[문제](https://programmers.co.kr/learn/courses/30/lessons/12928)
