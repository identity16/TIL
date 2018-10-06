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

## 접근제어자
default가 `private`임
- private
- protected
- public
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5OTc0OTAyMTEsMTcxOTY1OTIxLDgwOD
E5MDE1M119
-->