# HomeworkVIM_20203234
open source SW homework


----
## 1. Add quotes to ansible playbook
#### 1) 과제1 풀이
> G -> W -> i -> " -> end -> " -> esc -> ZZ
* G: 파일의 마지막 줄로 이동
* W: 스페이스 단위로 다음 글자로 이동
* i: 현재 위치에서 입력 모드 시작
* end: 라인 끝으로 이동
* esc: 일반 모드로 돌아옴
* ZZ: vim 저장 후 종료 **(=:x,:wq)**


#### 2) 과제1 풀이 gif
![1hh](https://user-images.githubusercontent.com/94359749/144551133-0bd64b48-8d9e-4f23-ad4b-f6258e8c92e2.gif)


----
## 2. simple replacements
#### 1) 과제2 풀이
> :%s/sublime\\|emacs/vim/g -> enter -> ZZ 

= sublime나 emacs이면 vim으로 String 치환
* :%s/change할 문자\\|change할 문자/change 문자
* g: 전체문장에 적용 (**없을 경우 line마다 1개 적용됨**)


#### 2) 과제2 풀이 gif
![2hh](https://user-images.githubusercontent.com/94359749/144551199-2456b3bf-3b73-4aad-83e1-46d80310a6e6.gif)


----
## 3. Satisfy the go linter
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
![3hh](https://user-images.githubusercontent.com/94359749/144551246-26aa27ee-1436-470b-ac14-100b6b3fee5c.gif)


----
## 4. Plotting some variables in python
#### 1) 과제4 풀이
> :%s/y1/abs(y1) -> enter -> :5s/1/4/g -> enter -> :4s/1/3/g -> enter -> :3s/1/2/g -> enter -> /k -> enter -> r -> b -> j -> r -> r -> j -> r-> g-> ZZ
* :%s/y1/abs(y1): y1 문자열을 abs(y1) 문자열로 String 치환
* :(바꿀 문자열이 있는 줄)s/change할 문자/change 문자: 그 줄에서 String 치환 ex) :5s/1/4/g: 5 번째 줄에서 숫자1을 모두 숫자 4로 바꿈
* /text : text 찾기 ex) /k: k 찾기
* r: 한글자를 바꿀 때 입력 모드
* j: 방향키 아래와 같음
* ZZ: vim 저장 후 종료 (=:x,:wq)


#### 2) 과제4 풀이 gif
![4hh](https://user-images.githubusercontent.com/94359749/144551307-3dafee61-090b-4476-b897-28418786c20a.gif)


----
## 5. Python dataclasses
#### 1) 과제5 풀이
> M -> k -> yw -> G -> b -> p -> a -> ,name,age,score -> esc -> ZZ
* M: 현재 화면 기준 중간으로 이동
* k: 방향키 위와 같음
* yw: 현재 word의 끝까지 복사
* G: 파일의 마지막 줄로 이동
* b: 단어 단위 뒤로 이동
* p: 현재위치 다음에 붙여넣기
* a: 현재 위치 다음 칸에서 입력 모드 시작
* esc: 일반 모드로 전환
* ZZ: vim 저장 후 종료 (=:x,:wq)


#### 2) 과제5 풀이 gif
![5hh](https://user-images.githubusercontent.com/94359749/144551348-ecc695bd-3194-4f6b-87a4-14a6f9cbbdd2.gif)


---
