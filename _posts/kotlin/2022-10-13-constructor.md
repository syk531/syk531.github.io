---
title: 생성자
author: syk531
date: 2022-10-13 04:40:00 +09:00
categories: [programming, kotlin]
tags: [programming, kotlin]
pin: true
---
kotlin에서는 클래스이름 옆에 소괄호를 붙여서 생성자를 만든다.   

### 생성자가 없을때
```kotlin
class NewsItemDto
```

```java
class NewsItemDto { }
```
kotlin에서는 class의 body가 없을 경우에는 java에서 처럼 {}로 감싸지 않아도 됨

### 인자가 없는 생성자
```kotlin
class NewsItemDto()
```
### kotlin에서의 인자가 여러개인 생성자

```kotlin
data class NewsItemDto (
   var title: String,
   var link: String
)
```
### java에서의 인자가 여러개인 생성자

```java
class NewsItemDto {
	String title;
	String link;
	
	NewsItemDto(String title, String link) {
		this.title = title;
		this.link = link;
	}
}
```