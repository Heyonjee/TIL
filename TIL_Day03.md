[Git & Github]
# TIL Day03

## CLI : Command Line Interface
- 가상 터미널 또는 터미널을 통해 사용자와 컴퓨터가 상호 작용하는 방식.
- 작업 명령은 사용자가 컴퓨터 키보드 등을 통해 문자열의 형태로 입력하며 컴퓨터로부터의 출력도 문자열의 형태로 주어진다.

## GUI : Graphic User Interface
- 사용자가 컴퓨터와 정보를 교환할 때 그래픽을 통해 작업할 수 있는 환경.
- 마우스 등을 이용하여 화면에 있는 메뉴를 선택하여 작업을 할 수 있다.

### CLI 명령어
- **mkdir** 폴더명/  => make directory, 폴더를 만든다.
- **cd** 폴더명  => change directory, 폴더를 이동한다.
- **touch** 파일명  => 파일을 만든다. 확장자 필수
- **ls**  => list segments, 해당 디렉토리 안의 파일들 리스트를 보여준다.
  - **ls -a**  : 숨김파일까지 전부 보여줌
  - **ls -l**  : 확장자 등 모든 정보를 표시해서 보여줌
- **rm** 대상  => remove, 대상을 삭제해준다, 휴지통이 아닌 바로삭제, 복구 안됨
(주의) 되도록 GUI 환경에서 삭제한다.
  - **r** : 재귀적으로 폴더 하단내역도 삭제
  - **rf** :  강제 삭제
- **mv**  => move
  - mv 대상파일 변경이름  : 이름을 변경
  - mv 대상파일 이동위치  : 파일을 이동
- **pwd**  => present working directory
  - 절대경로
  - 내 현재경로(사용자계정)에서 목적지에 도달하기 위해 거치는 모든 경로 표기
- **~**  => 물결표시
  - 상대경로
  - 현재 작업하고 있는 위치를 기준으로 목적지까지 도달하기 위해 거치는 경로 표기
- **..**  => 상위

### 기타
- 윈도우 환경 => C:/사용자(Users)/현재 사용자 계정
- **ctrl + l**  => 스크롤 이동
- **clear**  => 스크롤 이동, 위로 올라가서 이전 코드 확인하긴 어려움
- 화살표 위, 아래  => 이전 라인 가져오기

### Github 사용방법

#### commit 생성 
1. mkdir 폴더명/ => 폴더만들기
2. git init     => git이 버전관리 시작(처음 1번만 한다.)  
3. touch 파일명  => 파일만들기  
4. git status    => 파일상태(untracking) 
5. git add       => 파일 staging area로 올림
6. git status    => 파일상태(new file)
7. git commit -m "메시지 옵션"
8. 파일 수정 및 저장
9. git add
10. git commit -m "메시지 옵션"

#### push
1. new repository 생성
2. git remote add origin 원격 URL
3. git remote -v  =>조회해보기
4. git push origin master
