# Class
## 선언
```cpp
class IntSample {
public:
    void showScore();
    void setScore(int score);
    int getScore();

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
> 생성자는 어떻게 하지?

## 접근제어자
default가 `private`임
- private
- protected
- public
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NTM4MTc5NTUsODA4MTkwMTUzXX0=
-->