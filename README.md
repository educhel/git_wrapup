# Git 기초 정리

`Git` = 버전 관리 프로그램
-> 변경사항을 기록하는 역할을 한다.

## 설정
> 컴퓨터 한대 당 딱 한 번만 하면 됩니다.
시작에 앞서, 내가 누군지 알려 줘야 합니다.
```bash
git config --global user.name "유저명"
git config --global user.email "깃허브 가입 이메일"
```

```bash
git config --global init.defaultBranch main
```
기본 브랜치를 main으로 설정  
버전에 따라, master가 기본인 설정도 있기 때문에 이를 공통적으로 가져가기 위해서 설정

## Git 기초
- git의 3요소
  - working directory : 작업공간, 분장실
  - staging area : 대기공간, 무대 위
  - repositoty : 버전이 기록되는 공간, 사진들

```bash
git init 
```
일반 디렉토리를 git이 버전관리 할 수 있는 repository로 만든다.
-> 저장소 당 딱! 한번만 하면 된다.

### Local Repository
> 목적
1. 3공간을 넘나들기 위해 명령어 사용
2. 나의 상태 / 기록 내역을 확인하기 위해 사용

#### 목적 1
1. working directory -> staging area
```bash
git add 파일명
git add 폴더명
git add .
```

2. staging -> repository
```bash
git commit -m "변경사항을 기록하는 이유"
```

#### 목적 2
1. 파일의 상태를 확인
```bash
git status
```

1. 변경사항의 내역을 확인
```bash
git log --oneline
```