----------------------------------------------
git help : 커맨드 설명

working directory:
- 프로젝트 디렉토리

staging area:
- gid add 파일들 존재 영역

repository
- working directory 변경 이력 저장.

status(상태)
- Untracked 상태 : gid add 해주지 않은 상태
  
- Tracked 상태   : Git에 의해 변동사항 추적되고 있는 상태
  - Staged 상태  :  Staged(스테이징된,stage area에 올려진 상태)
  - Unmodified 상태 : 최신 커밋 모습과 비교했을 때 전혀 바뀐 게 없는 상태.
  - Modified 상태 : 최신 커밋 모습과 비교했을 때 수정된 상태.
![](https://velog.velcdn.com/images/chush4649/post/df0cab23-11f6-4428-a10d-74bf6cfeb75b/image.png)

Add the file : Untracked 상태의 파일을 처음으로 git add 해주면 Staged 상태.
Edit the file : 최신 커밋과 비교했을 때 차이가 없는 Unmodified 상태 파일 내용 수정. -> Modified 상태.
Stage the file : Modified 상태의 파일을 git add 해주면 -> Staged 상태.
Commit : 커밋을 하면 staging area에 있던 파일들 커밋 반영, -> 모든 파일들 Unmodified 상태.

----------------------------------------------
mkdir(file name) : 프로젝트 디렉토리 생성

cd (file name)/ : 파일 안으로 이동

git init : 디렉토리 버전 관리 
Initialized empty Git repository in /Users/choo/(file name)/.git/ -> 비어있는 레포지토리를 생성. 레포지토리 : 프로젝트 디렉토리의 각 버전이 담기는 저장소

ls -al : -a(all) 숨김 파일 포함 모든 파일 표시. -l(long) 파일의 상세 정보를 표시. 권한, 소유자, 그룹, 크기, 마지막 수정 날짜 및 파일 이름.

git config user.name "name"
git config user.email "name@gmail.com"
git commit -m "text" :
1.처음으로 커밋을 하기 전 사용자의 이름과 이메일 주소를 설정
2.커밋 메시지 남기기(옵션 -m)
3.커밋할 파일을 git add로 지정해주기

git add (file name) :
커밋할 파일을 미리 지정.
수정된 파일의 모습이 커밋에 포함될 것이라 지정하는 것!
프로젝트 디렉토리 내에 변경사항 생긴 파일을  staging area에 추가.

git add. : 현재 프로젝트 디렉토리 내에서 변경사항이 생긴 모든 파일들을 staging area에 추가.

git status : 변경사항 있는 파일상태 확인
----------------------------------------------
git reset : staging area에서 파일 제거
git add : staging area에서 파일 추가
git pull
git push
