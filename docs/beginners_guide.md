# 초보자용 사용 방법 
이 프로젝트는 프로그래밍을 잘 몰라도 기여가 가능합니다.  
첫 기여를 하고 싶다면 아래 내용을 따라해 보세요. 
* 이 문서는 2023년에 작성된 내용입니다. 개정이 필요하면 알려주세요 

## 오자 찾기, 또는 링크 추가시 {#find-misspelled-words-or-add-links}
웹사이트에서 오자를 찾으셨다면 docs폴더의 파일들을 열어봅니다.    
웹사이트에 링크를 추가하고 싶으시다면 docs폴더의 index.md파일을 클릭해서 열어봅니다.    
만약 원하는 부분을 찾으셨다면 이 프로젝트를 본인의 계정으로 fork해서 수정해야 합니다.

## 본인의 계정으로 Fork하기 {#fork-your-account}
Fork는 일종의 복사작업 입니다.  
우상단의 'Fork'버튼을 클릭합니다.  
!['fork'버튼](img/fork.png)  

Fork가 끝나면 본인의 깃헙 계정의 좌측상단에 저장소 이름이 표시됩니다. (phg9898대신에 본인계정이 표시되어야 합니다.)  
![fork가 끝나면](img/forked.png)  

이제 프로젝트가 본인의 계정으로 복사된 것입니다.  
이제부터 수정이 가능합니다.

## 저장소 클론하기
터미널을 열고 본 저장소의 URL을 자신의 기기에 클론합니다.

```bash
git clone "저장소 이름"
```

## 브랜치 생성하기 {#create-branch}
컴퓨터에 복사한 저장소 디렉토리로 이동합니다.

```bash
cd "파일 이름"
```

그리고 다음 명령어를 입력하여 브랜치를 생성합니다.
```bash
git checkout -b 브랜치 이름
```

예시:
```bash
git checkout -b add-readme-file
```

## 내용 수정하기 {#to-modify-the-content}

Fork된 저장소에서 수정할 파일을 찾아 클릭합니다. 
파일 내용이 표시되면 우측 상단의 연필 아이콘을 클릭하면 수정이 가능합니다.  
![edit](img/edit.png)  

오자를 수정하거나 링크를 추가합니다.  
링크를 추가할 때에는 기존의 링크 형식을 보고 동일한 포맷으로 적으면 됩니다.  
수정을 완료한 후에는 저장하기 위해 제일 아래의 'Commit changes'버튼을 누릅니다.  
![commit](img/commit.png)  

수정된 내용은 본인의 계정에 저장된 것 입니다. 이 수정사항을 원본 프로젝트에 반영하려면 풀리퀘스트(Pull Request)를 만들어야 합니다.

추가: 브랜치 생성 후 코드를 통해 변경할 시에도 비슷합니다. 변경하고자 하는 내용을 추가 혹은 수정하고 아래의 명령어를 통해 추가합니다.
예시:
```bash
git add Readme.md
```

그 후 commit 명령어를 통해 변경사항을 저장하고 푸시합니다.
예시:
```bash
git commit -m "Update Readme.md"
```

```bash
git push origin 브랜치 이름
```

## 풀리퀘스트 만들기 {#create-pull-request}
'Pull Requests'탭을 클릭합니다.  
![pr](img/pr.png)  

'New pull request' 버튼을 클릭합니다.  
![new_pr](img/new_pr.png)  

이제 풀리퀘스트가 만들어졌습니다. 원본 프로젝트의 관리자가 승인하면 반영됩니다.  

## 끝! {#end}
혹시 중간에 잘 안되는 부분이 있다면 인터넷 검색을 해보시고, 그래도 안된다면 phg98@naver.com으로 질문해 주세요.  
이제 첫 풀리퀘스트를 해보셨다면 [이슈페이지](https://github.com/phg98/hacktoberfestkorea/issues)로 가서 다른 적당한 항목이 있는지 확인해 보세요.  

### 참고 : 이 문서는 초보자를 위한 문서이므로 의도적으로 설명하지 않은 부분들이 있습니다. {#reference}
* 마크 다운 문법
  * [마크다운 기본 문법](https://www.notion.so/MD-Markdown-md-6f90928d5b8a4884b84a540410f8afdd)
  * [마크다운 확장 문법](https://www.notion.so/MD-Markdown-md-c990b53525f3443faa2dc0f292222407)
* 수정도중에 원본프로젝트의 변경사항 업데이트하기
* 커밋할때 좋은 메세지 작성하기
* Git 사용법 

천천히 하나씩 배워가시면 좋겠죠!
