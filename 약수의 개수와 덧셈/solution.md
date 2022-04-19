# 약수의 개수와 덧셈   

```swift
func solution(_ left:Int, _ right:Int) -> Int {
    var answer = 0
    
    for i in left...right{
        var count = 0
        
        for j in 1...i{
            if i % j == 0{
                count += 1
            }
        }
        
        if count % 2 == 0{
            answer += i
        }
        else{
            answer -= i
        }
    }
    return answer
}
```   

`for`문을 사용해 `left`에서 `right`까지 각각의 약수의 개수를 `count`에 저장한다.   
`count`가 짝수일 때 `answer`에 더하고, 홀수일 땐 뺀다.   

[문제](https://programmers.co.kr/learn/courses/30/lessons/77884)