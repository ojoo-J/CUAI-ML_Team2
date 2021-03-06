# CUAI 2020-2
머신러닝 2조 깃허브입니다

한국어 문서 추출요약 AI 경진대회
https://dacon.io/competitions/official/235671/overview/description/

[ BERT ] 

- 대용량의 unlabeled 모델을 미리 학습 시킨 이후에 특정 task를 가진 labeled data로 전이학습 하는 모델
- 기존에 NLP관련 모델들(OpenAI GPT, ELMO)의 경우는 대용량 unlabeled corpus를 통해 언어 모델을 학습하고, 이를 토대로 뒤쪽에 특정 네트워크를 따로 붙이는 형식을 사용하나, 이 방식들은 완전한 양방향 모델이라고 할 수 없다. 반면 BERT의 경우는 완전한 양방향 모델을 설계한 것에 의의가 있다. 
- BERT의 pre-train 방법론 
   (1) Masked Language Model
   - 입력 데이터 중 몇개에 마스킹(masking)을 하고 이를 transformer 구조에 넣어 주변      단어만 보고도 마스킹 된 단어를 예측하게 한다. BERT에서는 input 전체와 mask된         token을 한번에  transformer encoder에 넣고 원래 토큰을 예측하므로, 완전한 양방향     이 설계된 것. 
   (2) next sentence prediction 
   - 두 문장을 pre-training할 시에 같이 넣어 두 문장이 이어지는 문장인지 아닌지를 맞추     면서 학습을 진행 



[ reference ]

- 참고 논문 :  https://arxiv.org/pdf/1810.04805v2.pdf 
- 참고 블로그 1 :  참고 블로그1 
- 참고 블로그 2 : https://hwiyong.tistory.com/392 
- 참고 유튜브 (논문 리뷰방식 설명 ) : https://www.youtube.com/watch?v=vo3cyr_8eDQ 
