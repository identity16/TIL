# Struct
## 표기 방식
최근 버전에서는 `struct StructName variable`에서 `struct` 생략 가능

## 대입
같은 구조체 타입의 변수끼리 대입하면 멤버가 복사된다.
```cpp
struct {
	char Name[30];
	char MPhoneNum[20];
} Friend, Friend1;

...
Friend = Friend1;	// 가능!
...
```

> 같은 수, 같은 자료형을 가진 다른 구조체 타입의 변수 끼리도 가능?
> 위 예제처럼 배열이 있을 때는 Refernce가 복사됨?
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIyOTczOTE2Nl19
-->