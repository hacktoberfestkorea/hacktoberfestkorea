# 작업환경 구성하기

## 공통

아래 있는 모든 명령어는 cmd를 관리자 권한으로 실행 후 실행합니다

### GitHub 저장소 포크

```
phg98/hacktoberfestkorea --> [자신의GITHUB닉네임]/hacktoberfestkorea
```

## 작업환경 설정 - Local

### 작업하고싶은 폴더로 이동

```
(예시)
cd C:\Users\a0103\Documents\hacktoberfestkorea
```

### 저장소 복제

```
git clone https://github.com/[자신의GITHUB닉네임]/hacktoberfestkorea.git
```

git clone 명령어 사용시 repository에 있는 모든 내용이

```
C:\Users\a0103\Documents\hacktoberfestkorea
```

에 저장됩니다 이 경로는 **예시**이며 빌드시 원하는 경로를 직접 선택하시면 됩니다

### Python 설치

[점프 투 파이썬 - 파이썬 설치하기](https://wikidocs.net/8)

### Material for MkDocs 설치

```
pip install mkdocs-material
```

설치 완료시(예시):

```
Successfully installed livereload-2.6.3 lunr-0.5.8 markdown-3.2.2 mkdocs-1.1.2 mkdocs-material-6.0.1 mkdocs-material-extensions-1.0.1 pymdown-extensions-8.0.1
```

### 작업폴더로 이동

```
(예시)
cd C:\Users\a0103\Documents\hacktoberfestkorea
```

### 웹사이트 확인하기

```
mkdocs serve
```

명령어 실행후 [localhost:8000](localhost:8000)에 접속합니다

## 작업환경 설정 방법 - GitHub

### GitHub Actions 사용

GitHub Actions를 새로 만듭니다

[https://github.com/[자신의GITHUB닉네임]/hacktoberfestkorea/actions/new](https://github.com/[자신의GITHUB닉네임]/hacktoberfestkorea/actions/new)

에 접속해 **set up a workflow yourself**를 클릭합니다

```yml
name: ci
on:
  push:
    branches:
      - master
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-python@v2
        with:
          python-version: 3.x
      - run: pip install mkdocs-material
      - run: mkdocs gh-deploy --force
```

이 내용을 복사하고 **Start commit**을 클릭합니다</br>
잠시후 GitHub Actions가 작동하며 자동으로 **gh-pages** 브랜치를 생성하고,</br> 그 브랜치 안에 생성된 static page가 저장됩니다

### GitHub Pages 사용

GitHub 저장소 설정에 들어갑니다

[https://github.com/[자신의GITHUB닉네임]/hacktoberfestkorea/settings](https://github.com/[자신의GITHUB닉네임]/hacktoberfestkorea/settings)

하단에 있는 **GitHub Pages** 탭에서
Source를 None에서 gh-pages로 변경하고, 폴더를 /(root) 로 지정후 저장합니다

### 웹사이트 확인하기

[https://[자신의GITHUB닉네임].github.io/hacktoberfestkorea](https://[자신의GITHUB닉네임].github.io/hacktoberfestkorea)에 접속합니다
