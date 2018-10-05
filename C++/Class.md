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

> `new` 키워드 없이 객체 생성?
> 
> Java에서와 같은 생성자 함수는 어떻게 사용?

## 접근제어자
default가 `private`임
- private
- protected
- public
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcxOTY1OTIxLDgwODE5MDE1M119
-->