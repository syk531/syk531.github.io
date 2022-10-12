---
title: class와 data class 차이
author: syk531
date: 2022-10-13 04:00:00 +09:00
categories: [programming, kotlin]
tags: [programming, kotlin]
pin: true
---
class

```kotlin
class NewsItemDto (
    var title: String,
    var originallink: String,
    var link: String,
    var description: String,
    var pubDate: String
)
```
data class

```kotlin
data class NewsItemDto (
    var title: String,
    var originallink: String,
    var link: String,
    var description: String,
    var pubDate: String
)
```

class 앞에 data 키워드를 붙이게 되면 프로퍼티들에 대한 아래의 함수들이 컴파일 시점에 자동으로 생성된다.   
data를 보관하는 목적인 class에 사용한다.   
getter()   
setter()   
equals()   
hashCode()   
toString()   
copy()   