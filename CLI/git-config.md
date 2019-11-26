# Git Command Line Interface - Config

깃 터미널 명령어를 알아 보자

> 참고자료 : [git-scm](https://git-scm.com/book/ko/v1/%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-Git-%EC%B5%9C%EC%B4%88-%EC%84%A4%EC%A0%95)

## Git Config

- git 최초 설정
- git 설정 영역 지정 --global or --local

### 사용자 정보

```zsh
git config --global user.name "tester"
git config --local  user.name "tester"
```

- Git 설치 후 사용자 설정을 해야 한다
- 사용자의 정보는 Mac 같은 경우 access.app keychain 에 등록된다
- --global 옵션은 한번만 설정하면 전역에 저장된다
- 다른 사용자의 이름으로 커밋하고 푸쉬하고 싶을 때는 user.name / user.email 을 바꿔준다

### 편집기

```zsh
git config --global core.editor emacs
```

- 기본 편집기를 지정할 수 있다

### Diff 도구

```zsh
git config --global merge.tool vimdiff
```

- Merge 충돌을 해결하기 위해 사용하는 Diff 도구를 설정할 수 있다

### 설정 확인

```zsh
git config --list
```

- 설정된 값의 리스트를 노출한다
