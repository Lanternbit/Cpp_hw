# C++프로그래밍 11팀 과제 계획서

>과제명 : 

>팀명 : 11팀

>지도교수 : 컴퓨터공학과 심재창
<br/>

업무 분담   
|직책|이름|학과|학년|담당업무|
|----|----|---|----|-------|
|팀장|서경호|컴퓨터공학과|4학년|구현, 보고서 작성, 동영상 제작|
|팀원|김병현|컴퓨터공학과|3학년|구현, 보고서 작성, 동영상 제작|
|팀원|안보경|컴퓨터공학과|3학년|구현, 보고서 작성, 리플릿 작성|
|팀원|김선희|컴퓨터공학과|3학년|구현, 보고서 작성, 리플릿 작성|


## 1. 요약

### 1.1 과제 요약

#### &nbsp;컴퓨터로부터 이미지를 받아오고 출력하는 방식으로 틀린그림찾기 문제를 제시한다. 그림에서 차이점이 있는 부분을 픽셀단위로 위치를 지정해 '정답'으로 설정한다. 클릭 인식 범위를 지정해서 '정답' 위치에서 일정 범위를 클릭할 시 정답처리를 하는 방식을 이용해 C++로 틀린그림찾기 시스템을 구현한다.
<br/>

## 2. 개요

### 2.1 배경

#### &nbsp;틀린그림찾기는 오래된 게임으로 꾸준히 많은 사람들에게 사랑받고 있다. 이번 과제를 통해 C++를 이용하여 틀린그림찾기를 구현해 보았다.

### 2.2 필요성

#### &nbsp;틀린그림찾기는 지금 당장 검색하여 진행할 수 있는 누구나 아는 게임이다. 하지만 C++을 이용하고 학습하는 학생의 관점에서 봤을 때 이를 직접 구현해보는 것은 우리에게 필요한 좋은 경험이라 판단하였다. 이 프로젝트를 통해 C++을 사용하여 그림을 출력하고, 제한 시간, 정답 구역 설정 및 메인, 종료 화면 출력 등 게임의 기본적인 기능이나 구조를 조금조금씩 골고루 경험해볼 수 있을 것이다. 

### 2.3 선택 동기

#### &nbsp;회의결과 틀린그림찾기는 2장의 비슷한 사진을 배경으로 진행하기 때문에 여러 게임 중 결과물이 가장 직관적이고, 시각적으로 풍부할뿐만 아니라 재미도 있는 게임이라 판단하여 선택하게 되었다.
<br/>

## 3. 목표 및 내용

### 3.1 정량적/정성적 목표

>1) 정량적 목표 [항목 / 목표 / 방법]
>> - 응답시간 / 3초 이내 / ...<br>
>> - 사용자 만족도 / 90% / 사용자 설문조사<br>
>> - 틀린 부분 범위 정확도 / ...  / ...<br>
>> - 사진크기 / ...  / ... <br>

>2) 정성적 목표 [목표 : 평가방법]
>> - 게임성 : 게임의 컨셉 및 핵심적 재미 / 게임의 몰입도 / 게임 그래픽<br>
>> - 사업성 : 게임이 유료화 모델 / 게임 타깃 연령층 / 수익원의 다양성 / 게임의 개발일정 준수 가능성<br>
>> - 업무 완성도 : 업무의 양과 질 측면에서 직무 수행자에게 요구되는 수준을 초과/충족/미달/미흡/심각<br>
>> - 기한 준수도 : 해당 업무의 기한을 앞당김/준수함/준수하지 못함/심각함<br>
>> - 개선 노력도 : 업무개선 노력을 통해서 업무효율이 향상/기존의 방식 추구/부족/심각

### 3.2 과제 내용

#### 1) 메인 화면
- 시작 화면에 비교될 두 사진을 보여준다. 
- 좌측 맨 위, “틀린그림찾기”라는 문구를 표시한다. 
- 우측 하단, 남은 시간과 목숨을 나타낸다. <br>
![제한 시간](https://user-images.githubusercontent.com/50915637/169826113-a8add075-ef55-451e-a613-1444273cbd9b.PNG)
- 하단 중앙, “좌우에 틀린 곳을 찾아보세요.”라는 문구를 출력한다. 
- 바탕을 클릭하면 문구가 사라지고 게임이 시작된다. 

#### 2) 게임 중
- 좌우 그림 상관없이 틀린 부분을 클릭하면  체크 그림이 나타난다.<br>
![정답 체크](https://user-images.githubusercontent.com/50915637/169826109-cbc2fcb7-7e45-4d65-a6c8-eb7da304a43f.PNG)
- 잘못된 부분을 클릭하면 엑스 그림이 나타나고 목숨은 하나 줄어든다.<br>
![틀린 부분 체크](https://user-images.githubusercontent.com/50915637/169826115-c30a403c-8816-4ac0-acfb-a112e308ef13.PNG)

#### 3) 게임 종료 후
- 모든 틀린 부분이 체크되면 하단 중앙에 “성공, 다 찾았다!!!”라는 문장을 출력한다. 
- 남은 시간이 끝나거나 목숨이 남아있지 않을 경우, “실패..”라는 문장을 출력한다. 
<br/>

## 4. 결과물

### 4.1 예상 결과물

####  &nbsp;제한 시간 안에 화면에 보이는  두 그림을 비교하여 그림의 서로 다른 부분을 찾아 진행하는 게임으로 화면 아래에 스테이지 시간이 표시되어 남은 시간을 확인하며 게임을 즐긴다. <br>(스테이지가 진행됨에 따라 난이도를 높이기 위해 화면을 방해하는 장애물 구현 혹은 사진 화면 반전이 되는 게임이 만들어질 거라고 예상된다. )


![예상 결과물](https://user-images.githubusercontent.com/50915637/169825541-ca34a740-7b4d-403f-9715-8b9efbaecea6.png)
> 게임 중의 화면이다. 같은 듯 다른 그림 2장과 제한시간이 표시되어 있다.

### 4.2 기대효과 및 활용방안

#### &nbsp;본 게임은 스토리와 전략 등 정교한 것을 요구하는 다른 게임과 달리 단순하여 남녀노소 호불호 없이 누구나 쉽게 접근 가능하며 짧은 시간 내에 끝나 쉽게 질리지 않으며  중독성까지 있어 많은 사람들에게 사랑받을 수 있는 게임이다.<br> &nbsp;활용 방안으로는 학습 프로그램 중간 쉬어가는 타임으로 전 시간 배운 것들을 기반으로 한 그림을 사용한 틀린 그림 찾기 단계를 만들어 학습 흥미를 높일 수 있고, 사진을 넣어 만드는 게임 특성으로 이벤트성으로 친구, 가족의 원하는 사진을 의뢰받아 게임을 만들 수 있다. 호불호 없이 누구나 접근 가능하다는 게임의 특징을 살려 미술관 혹은 전시장에 게임 구현 가능 설치물을 준비해 눈으로만 그림을 감상하는 것이 아닌 직접 참여하며 즐겨 재미를 더할 수 있다. 더 나아가 활발한 시각 활동과 관찰력으로 뇌가 활성화돼 치매에도 예방이 된다.
<br/>

## 5. 수행일정

|                              |1주차|2주차|3주차|비고|
|------------------------------|-----|----|-----|----|
|1. 주제 선택                   |  O  |    |     |    |
|2. 업무 분담                   |  O  |    |     |    |
|3. 계획서 작성                 |  O  |    |     |    |
|4. 1차 구현, 시험              |     |  O  |    |    |
|5. 결과물 수정 및 완성          |    |  O  |     |    |
|6. 보고서 작성                 |     |     | O  |    |
|7. 발표PPT 및 리플릿 작성       |     |    |  O  |    |
|8. 동영상 제작                 |     |     |  O  |    |
<br/>

## 6. 참고문헌 및 자료

> [1] C++틀린그림찾기 구현(2020). https://m.youtube.com/watch?v=ln0GI6BzyII (accessed may 18,2022).
