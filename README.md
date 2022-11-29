# AIControl

|%s|%c|%d|%f|
|---|---|---|---|
|문자열(String)|문자 1개(character)|정수(Integer)|부동소수(floating-point)|



나의 첫번째 마크다운 파일입니다.

![KakaoTalk_20220822_163717510](https://user-images.githubusercontent.com/112088764/191095387-5c4d2a5c-2ced-4a74-aeba-10703fa0c6e9.jpg)


<header id="header">
<!-- 이력서 헤더 : 이름과 타이틀 작성 -->
  <h1>이태욱</h1>
  <hr>
     초보 개발자(Smart-Factory)
 <hr>
</header>
<main>
  <article id="mainLeft">
    <section>
      <h2>내이메일주소</h2>
      <!-- 소셜 미디어를 비롯한 연락처 정보 -->
      <p>
        <i class="fa fa-envelope" aria-hidden="true"></i>
        <a href="mailto:dlxo1107@gmail.com">dlxo1107@gmail.com</a>
      </p>
      <p>
        <i class="fa fa-facebook" aria-hidden="true"></i>
        <a href="dlxo1107@naveer.com">dlxo1107@naver.com</a>
      </p>
     
<section>
  <h2>내가배우는기술</h2>
  <!-- 자신이 잘할 수 있는 분야 -->
  <p>vim , Visual Studio Code   </p>
</section>
<section>
  <h2>학력</h2>
  <!-- 학력 -->
  <p>창원폴리텍대학교 - 스마트팩토리 재학중 (2022)</p>
  <p>창원공업고등학교 (2017-2020)</p>  
</section>
<section>
  <h2>나의 소개</h2>
  <!-- 자기 소개 -->
  <p>호기심 많고 무엇인가에 몰두하는 것을 좋아하며, 새로운 기술을 익히는 것을 주저하지 않는 도전자.</p>
</section>
<section>
  <h2>직장 경험</h2>
  <!-- 경력 작성 -->
  <p>직장경험은 없지만 폴리텍에서 취업하여 경험을 쌓을것이다.</p>
  
  <h3>수상 경력</h3>
  <ul>
   조만간 발명경진 대회에 나가 상을 탈 것이다.
  </ul>
</section>
손의 좌표를 [mediapipe](https://google.github.io/mediapipe/) 모듈로 손의 마디를 좌표로 인식한후  
인공지능(AI)으로 학습시켜서 램프를 키는 프로젝트입니다.

아래 유사 프로젝트들의 소스코드를 적극 활용하였습니다.

* [gesture-recognition by kairess](https://github.com/kairess/gesture-recognition)

# 프로젝트 실행 과정

학습
1. 데이터셋.py 를 실행시킨후 웹캠으로 0도 90도 180도에 대한 데이터셋을 만듭니다.
2. 머신러닝.ipynb를 순서대로 실행시켜 ai를 학습합니다.

실행
1. 웹캠과 아두이노를 연결한후 손가락 방향을 바꾸면서 각도가 바뀌면 램프가 바뀌는지 확인한다.
<img src="https://github.com/LETAUK/AIControlE/blob/main/img/0s.JPG" width="300" height="200">
<img src="https://github.com/LETAUK/AIControlE/blob/main/img/90s.JPG" width="300" height="200">
<img src="https://github.com/LETAUK/AIControlE/blob/main/img/180s.JPG" width="300" height="200">

# 각 구성파일의 역할

|파일명|설명|
|------|---|
|dataset폴더|데이터셋을 저장하는 폴더입니다|
|models.h5|학습시킨 AI 모델입니다|
|sketch_nov15a폴더|아두이노 파일입니다|
|데이터셋.py|데이터셋을 만드는 실행파일입니다|
|머신러닝.ipynb|AI학습을 시키는파일입니다|
|실행.py|AI를 실행시키는 파일입니다|

# 한계

* 손의 여러가지 각도는 인식이 되지 않는다  
* 검지손가락 이외의 손가락으로 가리킬시 손가락인식이 불가능하다
