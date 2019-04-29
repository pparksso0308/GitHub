## 충돌 해결 방법
### 1. 직접 해결
* 특정 branch 내용을 선택하거나 새로 작성하여 해결
* 충돌 부분 해결 후, 해당 파일을 add 명령을 사용해 staged 상태로 만듦 -> commit

### 2. Commit 메세지 내용을 자세하게 작성하기

### 3. 명령 사용
```c
// 현재 working 디렉토리의 파일 내용으로 최종 파일을 갱신함
git checkout --ours 파일이름

// Merge하는 branch에 있는 파일 내용으로 최종 파일을 갱신함
git chckout --theirs 파일이름 
```

## git branch 옵션들
```c
// 브랜치마다 마지막 커밋 메시지를 함께 보여줌
git branch -v

// 현재 checkout한 브랜치에서 이미 merge한 브랜치 목록을 확인할 수 있음
git branch --merged

//현재 checkout한 브랜치에서 merge하지 않은 브랜치 목록 확인 가능
git branch --no-merged

// 반드시 merge commit을 남기는 브랜치 
```
