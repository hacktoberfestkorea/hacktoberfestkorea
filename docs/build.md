# 설치방법

**모든 명령어는 cmd를 관리자 권한으로 실행 후 실행합니다**

### 1. Python 설치

[점프 투 파이썬 - 파이썬 설치하기](https://wikidocs.net/8)

### 2. Material for MkDocs 설치

```
pip install mkdocs-material
```

설치 완료시(예시):

```
Successfully installed livereload-2.6.3 lunr-0.5.8 markdown-3.2.2 mkdocs-1.1.2 mkdocs-material-6.0.1 mkdocs-material-extensions-1.0.1 pymdown-extensions-8.0.1
```

**MkDocs 파일을 새로 만들거나, 기존에 쓰던 파일을 다시 사용할수 있습니다.**

## 2.5 새로 MkDocs 생성

MkDocs 파일을 생성하고 싶은 폴더로 이동합니다.(예시)

```
cd C:\Users\a0103\myfolder
```

폴더 내에 MkDocs 파일 생성합니다.

```
mkdocs new .
```

파일 생성시 폴더 구조(예시):

```
myfolder
├─ docs/
│  └─ index.md
└─ mkdocs.yml
```

## 2.5 기존 프로젝트 다시 사용하기

MkDocs 폴더로 이동합니다.

```
cd C:\Users\a0103\Documents\hacktoberfestkorea
```

## 3. 웹사이트 미리보기

```
mkdocs serve
```

[localhost:8000](localhost:8000) 접속
