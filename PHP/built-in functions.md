Built-in Functions
===

## 문자열 조작
### strlen(\$string)
- 문자열 길이를 리턴
- 단, 한글의 경우 UTF-8에서 3바이트라서 원하는 결과가 나오지 않음
- => 이런 경우까지 제대로 처리하려면 `mb_strlen($string)` 사용

### substr(\$string, \$start_idx, \$len)

### str\_replace(\$search\_str, \$replace\_str, \$string)

### trim($string)

### htmlspecialchars(\$string, OPTION)
- HTML 문자 이스케이핑한 결과를 리턴
- 옵션
	- ENT_COMPAT : "만 변환 (default)
	- ENT_QUOTES : ', " 둘 다 변환
	- ENT_NOQUOTES : 변환 X

### strip_tags(\$string, \$allowed\_tags)
- 허용 태그는 "&lt;A&gt; &lt;FONT&gt;" 등의 문자열

### nl2br(\$string)

### implode(\$delimiter, \$array)
- 배열의 내용을 delimiter로 구분한 문자열 리턴
- join 함수와 동일(implode의 별칭)

### addslashes(\$string)
- SQL 문으로 동작할 만한 특수문자에 '\'를 붙여줌

### explode(\$delimiter, \$string)
- 문자열을 delimiter을 기준으로 나눈 배열 리턴

## 배열 조작
### list(\$var1, \$var2, \$var3..)
- `list($var1, $var2, $var3) = $array;` 와 같이 사용
- 앞에서부터 차례대로 배열에 있는 값을 변수에 할당
- 건너뛰고 싶은 부분에는 변수를 넣지 않고 `list(, , $var)`과 같이 쓰면 됨

### sort($arr)
### rsort($arr)

### assort(\$assoc_arr)
### arsort(\$assoc_arr)

### ksort(\$assoc_arr)
- 연관 배열의 키를 기준으로 정렬

### krsort(\$assoc_arr)
- 연관 배열의 키를 기준으로 정렬

### array\_merge(\$arr1, \$arr2..)
- 숫자 인덱스면 0부터 차곡차곡
- 연관 배열이면 그냥 합침
- 중복되는 키가 있는 경우, 덮어씀
- '+'와의 차이점
	- '+'는 중복되는 키가 있으면 덮어쓰지 않음
	- 숫자 인덱스라도 그대로 유지

### array\_slice(\$arr, \$start_idx, \$len)
- \$start\_idx와 \$len은 음수 가능

### array\_reverse(\$arr)