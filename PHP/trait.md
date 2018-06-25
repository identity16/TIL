Trait
===
코드를 재이용하기 위한 방법

## 정의 
 ```
 trait TraitName {
 	public function method1() {
	 	...
 	}
 	
 	private function method2() {
 		...
 	} 
 }
 ```
- `$this` 같은 키워드도 사용 가능

## 사용
```
class ClassName {
	use TraitName, TraitName2;
	...
}
```