# HomeworkVIM_20203234
open source SW homework


----
### 1. Add quotes to ansible playbook
#### 1) 과제1 풀이
> G -> W -> i -> " -> end -> " -> esc -> ZZ
* G: 파일의 마지막 줄로 이동
* W: 스페이스 단위로 다음 글자로 이동
* i: 현재 위치에서 입력 모드 시작
* end: 라인 끝으로 이동
* esc: 일반 모드로 돌아옴
* ZZ: vim 저장 후 종료 (=:x,:wq)


#### 2) 과제1 풀이 gif


----
### 2. simple replacements
#### 1) 과제2 풀이
> :%s/sublime\|emacs/vim/g -> enter -> ZZ
> sublime나 emacs이면 vim으로 String 치환
* :%s/change할 문자\|change할 문자/change 문자
* g: 전체문장에 적용 (**없을 경우 line마다 1개 적용됨**)


#### 2) 과제2 풀이 gif


----
### 3. Satisfy the go linter
#### 1) 과제3 풀이
> /V -> enter -> yw -> O -> //공백 -> esc -> p -> a -> TODO -> esc -> /D -> enter -> yw -> O -> //공백 -> esc -> p -> a -> TODO -> esc -> ZZ
* /text : text 찾기 ex) /V: V 찾기, /D: D 찾기
* yw: 현재 word의 끝까지 복사
* O: 현재 라인을 다음 줄로 밀고 입력 모드 시작
* p: 현재위치 다음에 붙여넣기
* a: 현재 위치 다음 칸에서 입력 모드 시작
* esc: 일반 모드로 돌아옴
* ZZ: vim 저장 후 종료 (=:x,:wq)


#### 2) 과제3 풀이 gif


----
### 4. Plotting some variables in python
#### 1) 과제4 풀이
> :%s/y1/abs(y1) -> enter -> :5s/1/4/g -> enter -> :4s/1/3/g -> enter -> :3s/1/2/g -> enter -> /k -> enter -> r -> b -> j -> r -> r -> j -> r-> g-> ZZ
* :%s/y1/abs(y1): y1 문자열을 abs(y1) 문자열로 String 치환
* :(바꿀 문자열이 있는 줄)s/change할 문자/change 문자: 그 줄에서 String 치환 ex) :5s/1/4/g: 5 번째 줄에서 숫자1을 모두 숫자 4로 바꿈
* r: 한글자를 바꿀 때 입력 모드
* j: 방향키 아래와 같음
