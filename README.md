# cp2-Recommendation-System

## 23.03.28 (화)
- [x] 추천 시스템에 대한 기본 지식 습득
- [x] 간단한 모델링 시도

<br/>

## 23.03.29 (수) - 1주차 주간보고 전체 피드백 내용
- 모든 변수가 똑같이 중요하다고 생각하면 안됩니다. 모든 변수가 똑같이 중요하지 않아요.
- 어떻게 하면 중요변수, 중요하지 않은 변수 판단할 수 있을가요?
- 아웃라이어(이상치), 아웃라이어의 기준은? box plot을 찾았다면? -> 제거 등... EDA, 분산값, 표준편차
- 시각화, 결측치 제거, 정규화 등...
- 모델들이 요구하는 사항들이 있습니다. 형식에 맞춰 input을 해야 합니다.
- 하이퍼 파라미터 - 조합식 -> Auto ML 사용. 더 중요한 것. 각각의 하이퍼 파라미터가 어떤 영향을 끼치는 지 알아야 한다.
- 모델 성능이 안좋으면 EDA 부터 다시 시작, 모델도 다시 찾아보고... 계속 반복 또 반복. -> 새로운 ML 탐색하기.
- 논문이 정리된 블로그를 볼 것.[Chat GPT가 잘 찾아 줄 것이예요]
- 딥러닝은 예측을 굉장히 잘 합니다. 유사도(실수-벡터) -> 딥러닝에게...
- 의사결정나무 성능이 아쉬워요(현장에서) -> 강점은 설명력이 강하다는 것.
- XAI 설명이 가능해야 합니다. 추천 시스템에 대한 이해도가 높아야 합니다. 


-  어떤 사람은 어떤 영화를 본다는 패턴을 발견할 수 있다.
-  취향을 고려하는 것은 movielens 데이터셋에서 찾기 어려울 수 있다. 평점밖에 없기 때문에.
-  오프라인 평가 모델(recall@k, pricision@k) -> 꼭 하셔야 합니다. 그래야 포폴에 넣을 수 있어요.

<br/>

## 23.03.31 (금)
- [x] EDA 및 KNN 정리
- [x] 공동 사용자가 file open할 수 있도록 코드 수정.
- [ ] '아이템 기반 최근접 이웃 협업 필터링으로 개인화된 영화 추천' 오류 확인 및 제거 (진행중)

<br/>

## 23.04.02 (일)
- [x] 1주차 작업한 내용에 대해서 피드백 진행


  **1. 수정 사항**
  - [ ] 데이터 사이즈 통일 부탁합니다. (one million size 디스코드 압축파일로 수령.)
  - [ ] 데이터 정의서 기록 부탁합니다. (초반에 넣어주세요.)
  - [ ] EDA(스토리텔링, 기승전결) 및 시각화 관련 피드백 부분 수정해주세요.
  - [ ] 서로의 데이터를 통합합니다.
  - [ ] 직업군별 연령의 분포, 성별의 분포 .. 와 같은 것을 확인. 보다 깊이 있게 EDA 부탁합니다. -> '우리가 이것을 모델에 적용시키겠다' 라는 시나리오가 필요합니다.
    
  **2. 주의 사항**
  - [ ] info() 같은 것은 굳이 하지 않아도 됩니다. (EDA단계에서는 주석을 한 줄, 한 줄 작성할 필요가 없다. plt같은 경우는 보면 알기 때문.)
  - [ ] 시각화 자료가 무엇을 의미하는 것인지에 대해서 기재.
  - [ ] 이것들을 왜 만들었고 왜 조합했는지, 어떻게 해석했는지 기재하면 더 도움이 된다.
  - [ ] 변수는 내가 만든 것이기 때문에. 왜 무엇을 만든 것인지 주석 기록해주시면 좋습니다.
    
  **3. 주간 보고서**
  - [ ] 옵션1 선택 완료.
    - 데이터 사이즈를 변경(모델의 정확도를 높이기 위해서) 합니다.
    - 모델에 연령대 & 직업군과 같은 변수를 추가해서 정확도가 높은 모델을 만들어 보고자 합니다.
  - [ ] 오프라인 미팅 내용 다루기. 
    - EDA 스토리라인이 부족, 시각화 자료를 다르게 구성해야 한다, 
    - 옵션1 선택에 따른 추가적인 EDA가 필요합니다. -> 피드백을 받았고 현재 수정중입니다. 
    - 해당 내용 수정 후 슬비님 코드와의 통합 및 변수를 추가한 모델링 예정. + 모델 고도화.
  - [ ] 프로젝트 기간 중 공통적으로 겪고 있는 어려움을 공유 (이 내용을 주간 보고서에 기록하는 것은 옵션입니다.)
    - 프로젝트 자체에 대한 고민보다는 프로젝트 기간 종료 후에 대한 고민. 이것을 포트폴리오로서 사용할 수 있을 것이며 완벽하지 않은 상태에서 취업(면접)을 준비하는 것이 맞는지, 아니면 공부를 더 진행한 다음에 취업을 하는 것이 맞는지(그렇게 되면 하반기 졸업생에게 밀릴 가능성이 있음) 에 대한 고민이 있다. 
    - DA를 희망하는 사람으로서 현재 SQL을 공부하고 있다(코딩테스트 및 포트폴리오 준비). 이것을 금번 프로젝트에 또, 포트폴리오에 어떻게 적용을 시켜야할지 방향성에 대한 고민이 있다. (어려움 공유)

- [ ] 23.04.04 (화) 15시까지 주간보고서(초안) 작성 후 공유바랍니다.
- [ ] 23.04.05 (수) ㅇㅇ님 휴가 예정입니다. 주간보고서 제출을 완료할 수 있도록 해주세요.
- [ ] 23.04.05 (수) EDA에 대한 2차 피드백이 진행됩니다. 조속한 마무리를 부탁합니다.
