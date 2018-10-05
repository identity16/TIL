# Dynamic Allocation
## 메모리 할당
`new` 키워드 이용
```cpp
...
int *pi = new int;
int *pj = new int[3];
...
```

## 메모리 해제
`delete`, `delete[]`(배열)
```cpp
...
int *pi = new int;
int *pj = new int[3];
...
delete pi;
delete[] pj;
...
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NTUyNDM4MTJdfQ==
-->