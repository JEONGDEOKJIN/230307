
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



git add 파일 이름
git add. : 모든 파일 스테이징
