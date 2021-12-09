## 작성 내용
git을 사용하며 자주 쓴 기능이나 헷갈리던 점들을 정리하여 추후 쓸 때 도움이 되도록 하려 한다.

### 커밋&푸쉬하는 방법
```
git status
git add <파일명1> <파일명2> <파일명3> 
git commit -m "<커밋 메시지>"
git push
```
이후 github 아이디 및 토큰을 입력하면 된다. add시 전부 넣고 싶다면 파일명 대신 '.'을 사용하고, add를 취소하고 싶다면 `git reset HEAD <파일명>`을 사용하자. 

만약 replit 사용 시 이전에 수정한 파일이 status에 잡힌다면 git pull을 활용하자. 이유를 모르겠지만 종종 파일이 제대로 저장되지 않는 것 같다.

### 비어있는 계정으로 커밋될 경우

```
git config --list
git config user.name "abcdefg"
git config user.email "abcd@efgh.ijk"
```

### 커밋을 잘못 해 지워야 할 경우

```
git log
git reset HEAD^
git push -f 
```
여러개를 지워야 할 경우 HEAD^ 뒤에 ~'숫자'를 달아주면 된다.


## 참고 자료

1. https://seonkyukim.github.io/git-tutorial/git-status/
2. https://curryyou.tistory.com/344  
3. https://0urtrees.tistory.com/44  
4. https://wellbell.tistory.com/43