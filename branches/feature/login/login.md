```shell
# -u 옵션: 새로운 기능 브랜치와 동일한 이름으로 중앙 원격 저장소의 브랜치로 추가한다.

// 로컬의 기능 브랜치를 중앙 원격 저장소 (origin)에 올린다.
$ git push -u origin feature/login branch

// -u 옵션으로 한 번 연결한 후에는 옵션 없이 아래의 명령만으로 기능 브랜치를 올릴 수 있다.
$ git push -origin feature/login branch
```

---
## 실제 연습
위에 있는 `git push -u origin feature/login branch` 명령어를 실제로 써보니까
`error: src refspec branch does not match any`라는 에러 문구가 뜨면서 안되길래 
그냥 `git push origin feature/login` 해봤음.

그러니까 아래와 같은 문구가 뜸.
```shell
PS C:\Users\USER\IdeaProjects\git-practice> git push origin feature/login
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'feature/login' on GitHub by visiting: # pull request 를 생성하라고 함.
remote:      https://github.com/djdjdddd/git-practice/pull/new/feature/login
remote:
To https://github.com/djdjdddd/git-practice.git
 * [new branch]      feature/login -> feature/login # feature/login 이라는 브랜치가 새롭게 생성됐다는 알려줌.
```