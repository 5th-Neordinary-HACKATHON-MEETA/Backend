#  MEETA (ETA)

> What's Your ETA? 대학생을 위한 회의 일정 관리 서비스
> 
> 🥉 5th Neordinary Hackathon 3rd Prize 🥉


 <br/>
 
![image](https://github.com/5th-Neordinary-HACKATHON-MEETA/Backend/assets/131960164/9634b8f4-b733-4299-a549-85f4dee2ec76)

<br/>

![image](https://github.com/5th-Neordinary-HACKATHON-MEETA/Backend/assets/131960164/4cb86c3d-bf23-45e5-a694-6f8acf85d19f)

<br/>

![image](https://github.com/5th-Neordinary-HACKATHON-MEETA/Backend/assets/131960164/29e8ce08-234b-4a30-bd6e-16e91e3546e7)

<br/>

![image](https://github.com/5th-Neordinary-HACKATHON-MEETA/Backend/assets/131960164/5507283e-bb68-4c4b-9905-cc0e15b57401)

<br/>

![image](https://github.com/5th-Neordinary-HACKATHON-MEETA/Backend/assets/131960164/d2ff0ed6-5336-4e87-aab5-fa1b94c9dbd8)

<br/>

![image](https://github.com/5th-Neordinary-HACKATHON-MEETA/Backend/assets/131960164/5e69a8b4-0338-48ab-8008-f4b6f7d783b9)


<h2> 주요 기능 </h2>
<details>
  <summary> 👨‍👩‍👧‍👦 팀</summary>
 <br/>
    1. 팀 생성하기
 <br/>
 <br/>
    2. 팀원 참여
  
 <br/>
</details>

<details>
  <summary> 🕒 회의</summary>
 <br/>
 1. 회의 생성 (팀장)
 <br/>
 <br/>
 2. 유저별 회의 가능 시간 설정 (팀원)
 <br/>
 <br/>
    3. 회의 시간 확정 (팀장)
 <br/>
 <br/>
    4. 회의 내에 공지사항 생성
</details>















## 협업 규칙
<details>
    <summary> 커밋 컨벤션</summary>
archivvonjang님의 [블로그](https://velog.io/@archivvonjang/Git-Commit-Message-Convention) 를 참고하여 정리하였습니다.
<br/>
<br/>


## Commit Message Convention

### 1. Commit Message Structure
-   기본적인 커밋 메시지 구조

    ```
      제목 (Type: Subject)
      (한줄 띄어 분리)
      본문 (Body)
      (한줄 띄어 분리)
      꼬리말 (Footer)
    ```

### 2. Commit Type
-  커밋의 타입 구성
  
    ```
      태그: 제목 
      (:space 제목으로 : 뒤에만 space를 넣는다.)
    ```
    <br/>
    
    |Tag Name|Description|
    |:--:|:--:|
    |Feat|새로운 기능을 추가|
    |Fix|버그 수정|
    |!BREAKING CHANGE|커다란 API 변경의 경우|
    |!HOTFIX|급하게 치명적인 버그를 고쳐야하는 경우|
    |Style|코드 포맷 변경, 세미 콜론 누락, 코드 수정이 없는 경우|
    |Refactor|Production Code(실제 사용하는 코드) 리팩토링|
    |Comment|필요한 주석 추가 및 변경|
    |Docs|문서 수정|
    |Test|테스트 코드 추가, Production Code(실제 사용하는 코드) 변경 없음|
    |Chore|빌드 업무 수정, 패키지 매니저 수정, 패키지 관리자 구성 등 업데이트, Production Code 변경 없음|
    |Rename|파일 혹은 폴더명을 수정하거나 옮기는 작업만인 경우|
    |Remove|파일을 삭제하는 작업만 수행한 경우|
    <br/>

    추가적인 문맥 정보를 제공하기 위한 목적으로 괄호 안에 적을 수도 있다.
    ```
      Feat(navigation)
      Fix(DB)
    ```

### 3. Subject
-  제목은 50글자 이내로 작성한다.
-  첫글자는 대문자로 작성한다.
-  마침표 및 특수기호는 사용하지 않는다.
-  영문으로 작성하는 경우 동사(원형)을 가장 앞에 명령어로 작성한다.
-  과거시제는 사용하지 않는다.
-  간결하고 요점적으로 즉, 개조식 구문으로 작성한다


```
EX)
Fixed --> Fix
Added --> Add
Modified --> Modify
```

### 4. Body
-  72 글자 이내로 작성한다.
-  최대한 상세히 작성한다. (코드 변경의 이유를 명확히 작성할수록 좋다)
-  어떻게 변경했는지보다 무엇을, 왜 변경했는지 작성한다.
<br/>

### 5. Footer
-  선택사항
-  자세한 건 블로그 참고
<br/>

### 6. Example

```
Ex1)
Feat: 회원 가입 기능 구현 ---> Commit Type

SMS, 이메일 중복확인 API 개발 ---> Body

Resolves: #123 ---> Footer (선택 사항항)
Ref: #456
Related to: #48, #45

Ex2)
!BREAKING CHANGE: 게시글 작성 API 변경

게시글 작성 시 참여자 초대의 ~~ 부분에서 프론트에 데이터를 정확하게 응답하기 위해 ~~한 부분을  ~~하게끔 변경한다.
```
<br/>

커밋 메시지를 여러 줄 입력하려면??
```
git commit -m "커밋메시지 입력
~~~
~~~
```
위처럼 따옴표를 닫지 않고 계속 입력하면 된다.

<br/>


그 외 자주 쓰이는 예시
```
  Fix : 버그 수정                                                   ---> Commit Type
  Fix my test                                                       ---> Body
  Fix typo in style.css
  Fix my test to return undefined
  Fix error when using my function

  Update : Fix와 달리 원래 정상적으로 동작했지만 보완의 개념       ---> Commit Type
  Update harry-server.js to use HTTPS                             ---> Body

  Add                                                             ---> Commit Type
  Add documentation for the defaultPort option                     ---> Body
  Add example for setting Vary: Accept-Encoding header in zlib.md

  Remove(Clean이나 Eliminate) : ‘unnecessary’, ‘useless’, ‘unneeded’, ‘unused’, ‘duplicated’가 붙는 경우가 많음 ---> Commit Type
  Remove fallback cache                                                                                       ---> Body
  Remove unnecessary italics from child_process.md

  Refactor : 리팩토링                                                   ---> Commit Type

  Simplify : Refactor와 유사하지만 약한 수정, 코드 단순화                 ---> Commit Type

  Improve : 호환성, 테스트 커버리지, 성능, 검증 기능, 접근성 등의 향상     ---> Commit Type
  Improve iOS's accessibilityLabel performance by up to 20%               ---> Body

  Implement : 코드 추가보다 큰 단위의 구현                                 ---> Commit Type
  Implement bundle sync status                                             ---> Body

  Correct : 주로 문법의 오류나 타입의 변경, 이름 변경 등에 사용             ---> Commit Type
  Correct grammatical error in BUILDING.md                                 ---> Body

  Prevent                                                                 ---> Commit Type
  Prevent hello handler from saying Hi in hi.js                           ---> Body

  Avoid : Prevent는 못하게 막지만, Avoid는 회피(if 등)                     ---> Commit Type
  Avoid flusing uninitialized traces                                       ---> Body

  Move : 코드나 파일의 이동                                                 ---> Commit Type
  Move function from header to source file                                 ---> Body

  Rename : 이름 변경                                                       ---> Commit Type
  Rename node-report to report                                             ---> Body
```

### 7. Emoji
-    이슈를 파고, 글 내용에다가 아래의 이모지와 함께 어떤 것을 할지 자세히 적는다.
<br/>
🎨	코드의 형식 / 구조를 개선 할 때<br/>
📰	새 파일을 만들 때<br/>
📝	사소한 코드 또는 언어를 변경할 때<br/>
🐎	성능을 향상시킬 때<br/>
📚	문서를 쓸 때<br/>
🐛	버그 reporting할 때, @FIXME 주석 태그 삽입<br/>
🚑	버그를 고칠 때<br/>
🐧	리눅스에서 무언가를 고칠 때<br/>
🍎	Mac OS에서 무언가를 고칠 때<br/>
🏁	Windows에서 무언가를 고칠 때<br/>
🔥	코드 또는 파일 제거할 때 , @CHANGED주석 태그와 함께<br/>
🚜	파일 구조를 변경할 때 . 🎨과 함께 사용<br/>
🔨	코드를 리팩토링 할 때<br/>
☔️	테스트를 추가 할 때<br/>
🔬	코드 범위를 추가 할 때<br/>
💚	CI 빌드를 고칠 때<br/>
🔒	보안을 다룰 때<br/>
⬆️	종속성을 업그레이드 할 때<br/>
⬇️	종속성을 다운 그레이드 할 때<br/>
⏩	이전 버전 / 지점에서 기능을 전달할 때<br/>
⏪	최신 버전 / 지점에서 기능을 백 포트 할 때<br/>
👕	linter / strict / deprecation 경고를 제거 할 때<br/>
💄	UI / style 개선시<br/>
♿️	접근성을 향상시킬 때<br/>
🚧	WIP (진행중인 작업)에 커밋, @REVIEW주석 태그와 함께 사용<br/>
💎	New Release<br/>
🔖	버전 태그<br/>
🎉	Initial Commit<br/>
🔈	로깅을 추가 할 때<br/>
🔇	로깅을 줄일 때<br/>
✨	새로운 기능을 소개 할 때<br/>
⚡️	도입 할 때 이전 버전과 호환되지 않는 특징, @CHANGED주석 태그 사용<br/>
💡	새로운 아이디어, @IDEA주석 태그<br/>
🚀	배포 / 개발 작업 과 관련된 모든 것<br/>
🐘	PostgreSQL 데이터베이스 별 (마이그레이션, 스크립트, 확장 등)<br/>
🐬	MySQL 데이터베이스 특정 (마이그레이션, 스크립트, 확장 등)<br/>
🍃	MongoDB 데이터베이스 특정 (마이그레이션, 스크립트, 확장 등)<br/>
🏦	일반 데이터베이스 별 (마이그레이션, 스크립트, 확장명 등)<br/>
🐳	도커 구성<br/>
🤝	파일을 병합 할 때
</details>
