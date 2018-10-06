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


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM5OTE5MjExMSwxNzE5NjU5MjEsODA4MT
kwMTUzXX0=
-->