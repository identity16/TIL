`Require` / `Include`
===
다른 파일을 읽을 때 사용

### 공통점
- require과 include 모두 같은 기능을 한다.
- 다른 파일의 코드를 require/include 문 위치에 넣는 느낌인 듯(Scope도 적용되고..)
- 경로는 PHP 설정(php.ini)의 include_path에서 우선적으로 찾음
- include_path에 없으면 현재 디렉터리에서 탐색
- include_path에 여러 경로를 지정하고 싶으면 구분자 사용
	- 구분자 : `;`(Windows), `:`(Mac, Linux)
	- Example : `include_path = ".:/Applications/XAMPP/xamppfiles/lib/php`

#### 리턴 값
- 포함하는 파일의 리턴 값 또는 포함 성공 여부에 따라서 TRUE, FALSE

### 차이점
 오류 발생 시,
 
- include : Warning을 출력, 처리 실행
- require : Fatal Error, 처리 정지

### `require_once`, `include_once`
- require, include를 여러 번 시도해도 단 한 번만 실행함

