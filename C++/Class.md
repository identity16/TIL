# Class
## 선언
```cpp
class IntSample {
public:
    void showScore();
    void setScore(const int score);

private:
    int score;
}

void IntSample::showScore() {
    ...
}
...
IntSample obj;		// 객체 생성
...
```

> `new` 키워드 없이 객체 생성? => ㅇㅇ 저렇게 하면 생성자가 호출됨
> 
> Java에서와 같은 생성자 함수는 어떻게 사용? => 생성자 오버라이딩, 파라미터 전달도 가능(`IntSample obj(p1, p2);`)

## 접근제어자
default가 `private`임
- private
- protected
- public

## 복사생성자
생성자 인자로 객체를 넣어주면 멤버변수를 복사해서 새로운 객체 생성

## 소멸자
`~ClassName();` 형태

## `new`
new 연산자로 객체를 생성하면 객체의 주소를 넘겨주기 때문에 포인터 변수로 받아야 한다.

## `&` 타입
기존 변수에 새로운 별명을 추가하는 느낌?
```cpp
int x = 100;
int &Y = x;
Y = 200;	// now, x = 200
cout << x;	// prints 200
```

## `this`
객체 자신의 **포인터**

## 프렌드 함수
특정 클래스와 친분 관계를 허락하여 `private` 멤버를 참조할 수 있음
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MTUwOTgwODcsMTM5OTE5MjExMSwxNz
E5NjU5MjEsODA4MTkwMTUzXX0=
-->