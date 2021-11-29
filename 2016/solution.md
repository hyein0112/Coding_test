# 2016
```swift
func solution(_ a:Int, _ b:Int) -> String {
    
    let days = ["SUN", "MON", "TUE", "WED", "THU", "FRI", "SAT"]
    let monthDay = [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
    
    var day = 5
    
    for i in 0..<a-1 {
        day += monthDay[i]
    }
    day += b-1

    day = days[day%7]
    
    return days[day%7]
}
```   
요일과 각 월의 일 수를 각각 `days`와 `monthDay`배열로 선언  
2016년은 윤년이므로 2월달의 일 수를 29로 선언한다.  
2016년 1월 1일은 금요일이므로 `day`를 5로 선언   
`for`문을 사용해 `a-1`월 까지 더한 후 `b-1`만큼 일 수를 더해 7로 나눈 값이 `a`월 `b`일의 요일이 된다.
