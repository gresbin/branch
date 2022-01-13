## git branch

### git branch 명령어

* 브랜치 생성, 삭제, 조회

  ```bash
  # 브랜치 조회 - *이 붙어있는 브랜치가 현재 작업하고 있는 브랜치
  $ git branch
  
  # 원격저장소의 브랜치 조회
  $ git branch -r
  
  # 브랜치 생성(작업할 내용에 맞는 브랜치 명 작성)
  $ git branch {생성할 브랜치 명}
  
  # 브랜치 삭제
  # 수정된 내용을 머지하고 난 후에 삭제 가능
  $ git branch -d {생성한 브랜치 명}
  
  # (주의) 병합되지 않은 브랜치 강제 삭제
  $ git branch -D {생성한 브랜치 명}
  ```

  

### git switch

* 현재 브랜치에서 다른 브랜치로 head를 이동시키는 명령어

* head는 현재 브랜치를 가리키는 포인터

  ```bash
  # 다른 브랜치로 이동
  $ git switch {이동하려고 하는 브랜치 이름}
  
  # 브랜치를 새로 생성하고 동시에 이동
  $ git switch -c {생성할 브랜치 이름}
  ```

  

* **주의 사항**

  git switch하기 전에 commit을 했는지?