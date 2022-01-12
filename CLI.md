# **CLI**

## GUI vs CLI

1. GUI (Graphic User Interface)
   * 그래픽을 통해서 사용자와 컴퓨터가 상호작용하는 방식
2. CLI(Command Line Interface)
   * 터미널을 통해 사용자와 컴퓨터가 상호작용하는 방식



## CLI를 사용하는 이유

new라는 폴더를 만들고자 한다면?

1. GUI에서는 -> 우클릭 -> 새로만들기  -> 폴더 -> new
2. CLI에서는 -> `mkdir 폴더명 ` (폴더생성) -> `mv 파일명 / 폴더명`(파일을 해당 폴더로 옮기기)



## 작업 위치 (경로)

### 루트 디렉토리(/)

* window의 경우 일반적으로 c드라이브를 의미

### 홈 디렉토리(~)

#### 	상대 경로

* ./ : 현재 작업하고 있는 폴더
* ../ : 현재 작업하고 있는 폴더의 상위 폴더





## 명령어

**cd** :  작업중인 디렉토리를 옮길 때 사용

``` bash
$ cd
-> 홈 디렉토리로 이동
$ cd folder # tab 으로 자동완성
$ cd .. 
-> 상위 폴더로 이동
```

 

**ls** : 현재 작업중인 디렉토리의 폴더 / 파일 명을 보여주는 명령어

```  bash
# 기본 사용
$ ls

# all
$ ls -a

# long
$ ls -l

# all , long 동시 사용
$ ls -a -l
```



**mkdir** : 폴더를 생성하는 명령어 / 폴더 이름 사이에 공백을 넣고싶다면 따옴표로 묶어서 입력

``` bash
$ mkdir folder folder1

# 공백이 필요한 경우
$ mkdir "2022년 1월 12일"
```



**touch** : 파일을 생성하는 명령어(폴더 생성과 방법 동일) / .을 폴더or파일명 앞에 붙이면 숨김폴더or파일로 생성

```bash
$ touch test.txt

# 실행 시
window = start
mac = open
```



**rm** : gui의 경우 휴지통으로 보내지만 cli의 경우는 shift+delete랑 같음

```bash
# 폴더 삭제 시
$ rm -r folder명 /

# 파일 삭제 시
$ rm test.txt
```

**mv** : 파일이나 폴더 이동시킬 때

```bash
$ mv (이동시킬 파일or폴더) (이동할 폴더)
$ mv (변경시킬 파일or폴더) (변경할 이름)
```

