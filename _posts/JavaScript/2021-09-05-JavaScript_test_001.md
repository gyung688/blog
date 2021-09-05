---
layout : post
categories : JavaScript
title: [자깨]자바스크립트에서의 객체
excerpt: 자바스크립트에서의 객체에 대해 이해해보자.
---

코디 린들리의 "자바스크립트를 깨우치다"를 읽고 작성했습니다.  

-------------------------------------
자바스크립트는 객체를 사용해 값을 표현한다.   
다음은 사용자 정의 객체와 네이티브 객체이다.

사용자 정의 생성자  
Person() 객체를 만들기 위해 Person 생성자 함수를 정의한다.  

```JavaScript
    var Person = function(living){
        this.living = living;
        this.age = age;
        this.gender = gender;
        this.getGender = function() {return this.gender};
    }
```

Person 객체의 인스턴스를 만들고 cody라는 변수에 저장한다.
```JavaScript
    var cody = new Person(true, 33, 'male');
    
    console.log(cody);
```
네이티브 객체는 바로 인스턴스를 만들어 문자열을 사용한다.  
문자열 객체의 인스턴스를 만들어 myString 변수에 저장한다.
```JavaScript
    var myString = new String('foo');
    console.log(myString);
    }
```

Person과 문자열 생성자를 보면 둘의 사용 패턴이 동일함을 알 수 있다.



[출처] 자바스크립트를 깨우치다
