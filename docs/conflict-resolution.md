# Conflict Resolution Log

## 충돌 기록 #1 (자명한 충돌)
### 참여자
- 작성자 star-candy(신희수)
- 기준 branch : feature/trivial-conflict-a
- 참여 branch : feature/trivial-conflict-b

### 자명 충돌이란?
- 두 개 이상의 브랜치에서 동일한 파일의 같은 줄을 다르게 수정하고 병합(Merge)을 시도할 때 발생

### 상황(What happened)
- 자명충돌 관련 문서 작성을 위해 feature/trivial-conflict-a branch를 생성함 (a)
- 비자명 충돌 문서 작성을 위해 feature/trivial-conflict-b branch를 생성함 (b)
- branch a에서 docs/conflict-resolution.md 문서를 수정 및 push
- branch b에서 동일 영역을 수정 및 push
- branch b에서 a로 merge하기 위해 pr시 conflict 발생


### 진행 경과
- main을 부모로 하는 feature/trivial-conflict-a branch 생성
- feature/trivial-conflict-a branch를 부모로 하는 feature/trivial-conflict-b branch 생성
- a branch에서 docs/conflict-resolution.md 문서 자명충돌 템플릿 생성 
- 원격으로  push
- b branch에서 docs/conflict-resolution.md 문서 비자명충돌 템플릿 생성 
- 원격으로 push
- b branch에서 a branch로 merge 위한 pr 요청시 자명충돌 발생
- ![alt text](../images/conflict1.png)
- ![alt text](../images/conflict2.png)

### 충돌 내용(Conflict markers)
- ![alt text](../images/conflict3.png)
- 3가지 해결방법 제시됨
    - 현재 branch (b) 내용 수락
    - 기존 branch (a) 내용 수락
    - 두 branch 변경 내용 모두 수락

- 자명충돌을 먼저 실습 후 문서화 하는 것이 목적
    - 따라서 a branch 내용을 남기는 방식으로 conflict를 해결함
    - accept incoming change
- ![alt text](../images/conflict4.png)

#### 충돌 마커는 무슨 의미인가?
```
<<<<< : pr을 보낸, 즉 merge 요청을 보낸 branch (b) conflict 발생 부분을 보여줌

===== : 두 branch 사이를 나누는 구분점

>>>>>> : pr을 받은, 즉 merge 요청을 받은 branch (a) conflict 발생 부분을 보여줌

```

------