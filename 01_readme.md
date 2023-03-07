

- 아래 내용 중 중요한건 옵시디언에 정리했음. 

--- 
## 마크다운 이란? 

<!-- 마크 다운이란?  -->
- 깃헙 문서, 등에 올릴 수 있음. 
- 테스트

<br>


<!-- 문서 제목
        # 으로 작성 -->
# 230307 
## 샵 2개 제목
### 샵 3개 제목 
#### 샵 4개 제목


<!-- -- 으로 리스트 작성 -->
--- 

# git 프로젝트 

<br>

## git 이란? 
- 형상 관리 도구 중 하나 
- 형상 관리 도구란 '버전 관리 시스템' 
    ex) 버전 1, 버전 2, 등등 
- 작업하면서, 작업의 리스트를 관리할 수 있다. 
- ⭐⭐⭐ 잘 써보자!!! 
    - 이걸로 반복해서 공부할 수 있을 것 같음.

<br>

## git 의 장점 
- 협업하는 단계에서 소스 코드 파일을 주고 받을 필요 없이, 같은 파일을 팀원과 병렬로 작업이 가능
ex) 내가 class 추가 했어. / 나도 여기 추가 했어. / 수정 을 일일이 확인하는게 번거로움 -> so, 어디를 어떻게 병합하는지 등을 알려주는데 편함 
- 눈으로 보고 찾는 것 보다, 효율이 좋고, 작업이 편함 
- 코드의 다른 부분을 바로 찾을 수 있다. ⭐⭐⭐ 
- 얼마나 성실하고, 뭘 했고를 알 수 있어 ⭐⭐⭐⭐⭐⭐⭐⭐⭐⭐⭐⭐ 
    - 블로그와 같이 쓰면 돼 ⭐⭐⭐⭐⭐⭐ 
    - ⭐⭐⭐⭐⭐ 매일 1커밋 하자 ⭐⭐⭐⭐⭐ 

<br>

## 깃헙 가입 및 설치 
- https://github.com/ 

<br>

## 깃 설치 
- https://git-scm.com/download/win

<br>

## git 열기  
1. 윈도우 탐색창에서 git bash 검색 
2. vscode 에서 `cntrl ~` 누르면 터미널 열림 -> 여기에서 -> 추가 

## git 사용자 설정 
- 닉네임 및 이메일 설정
`git config --global user.name "본인 깃허브 닉네임"`
`git config --global user.email "본인 깃허브 이메일"`
- 설정 여부 조회 
`git config --global --list`

<br>

- 내꺼 기입 ✅✅✅✅✅ 
`git config --global user.name "JEONGDEOKJIN"`
`git config --global user.email "anotheryear.hm@gmail.com"`

<br>

- 요런식으로 나옴 
`user11@DjDragon MINGW64 ~
$ git config --global --list
user.name=JEONGDEOKJIN
user.email=anotheryear.hm@gmail.com`

## git 저장소 초기화 저장소를 생성하는 명령어
- 해당 프로젝트 경로에서 `git init` 작성
- `cd ..` : cd 하고 - 한칸 띄고 - .. / 한 폴더 뒤로 이동 
- `ls -a` : 경로의 파일을 전부 보고 싶을 때 
- `cd 폴더명` : 해당 폴더로 경로 이동
- `tab` : cd 앞 부분 폴더명 쓰고 기억 안나면 -> tab -> 나머지 자동 완성
- `화살표 윗 키` : 앞에서 쓴거 찾아서 쓰기 


## git graph 설치 
- vs code extension 에서 설치하면 됨 

<br>

## github 에서 보이는거 대로 해보기

echo "# 230307" >> README.md
- `git init`
    % 저장소가 생김
    % 색깔이 바뀌면 - 저장소와 파일 내용이 다르다는 것 임. 
    % 추가되면 : 녹색 / 삭제하면 : 빨강

    % ⭐ 1) cd 명령어 써서 내가 저장하고 싶은 '폴더'로 가야 함 / 오늘 날짜 폴더로 하면 좋을듯
    % ⭐ 2) 그 다음 `git init` 

- `git add README.md`
    % 일단 무시 

git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/JEONGDEOKJIN/230307.git
git push -u origin main



## 올리는 법
git 저장소 파일 스테이징
업로드전 준비 업로드할 파일들

% 커맨드로 작성
git add 파일 이름
git add. : 모든 파일 스테이징

% 깃 그래프로 올릴 수도 있음. 


## 커밋 메시지 
- 1. git commit -m "메시지 내용" 작성 
- 2.  위에 커밋버튼 위에 
- 이렇게 하면 파일 올릴 준비가 끝남. 

## 실제 저장소에 연결하려면 
- 원격 저장소에 연결하기 
- `git remote add origin https://github.com/JEONGDEOKJIN/230307.git` 
(이건 깃헙 설명에 있음!) (https://github.com/JEONGDEOKJIN/230307)

- 업로드 할 때 
`git remote add origin 업로드할 주소` 

- git push ⭐⭐⭐⭐⭐ 
    - 원격 저장소에 업로드 하기 
`git push -u origin main`
-지금은 main 이 아니라, master 로 함 ✅✅ (앞에서 뭐 해줬어야 하나봐)
- ❓❓❓ 안 올라가는데? 

## 사용자 명이 다를 경우
- 깃 관리하면서, 자리 이동했을 때, 사용자 명이 다를 경우
- 제어판 -> 사용자 계정 -> 자격증명관리자 -> 윈도우 자격증명 관리자 탭 -> github.com 탭 열고 -> 해당 탭 '제거!' ⭐⭐⭐⭐⭐ -> 다시 사용자 등록 하기 (이름 & 아이디)

## 협업 할 때 주의할 것
- 협업 할 때, git 에 push 부터 날리면 안 되고
- A,B 가 있으면 -> A가 먼저 PUSH -> B가 A 의 작업물을 `병합`하지 않고 PUSH 하면, A 의 작업물이 다 날아감. 
- 무작정 PUSH 하면 안 돼
- 작업물을 올릴 때는

## git 파일 잘못 만들었을 때 
`rm -rf .git/` : 해당 폴더 삭제  

## 새로운 환경에서 git 저장소 연결 할 때~ 

1. git init
2. git remote add origin "저장소의 주소" 
- 저장소 주소는 해당 깃헙 저장소에 접속해서, code 초록색 버튼, 누르면 나옴 

## 무조건 pull ->  push ⭐⭐⭐⭐⭐ 의 순서로 해야 함. 


## 오늘 과제 
- 지금까지 한 과제, 수업 자료, 저장소 만들어서, 업로드 하기 ✅ 