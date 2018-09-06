## 2Sum

```swift
func 2Sum(array:[Int], _ target: Int)->(Int,Int) {
    var dic: Dictionary<Int,Int> = [:]
    for (i,num) in array.enumerated() {
        if let lastIndex: Int = dic[target - num] {
            return (i,lastIndex)
        }else {
            dic[num] = i
        }
    }
}
```

