<div align="center">
  <h1> 🍿 영화 리뷰 감성 분석 </h1>
  <br>
  </div>
  
  ## 프로젝트 개요 
  - 📅 프로젝트 기간 : 2021.11.08 - 2021.11.11   
  - 프로젝트 목표 : 리뷰의 감성분석을 통해 영화에 대한 긍정/부정의 비율을 확인 할 수 있음
  <br>
  
  ## 프로젝트 과정 
  - 데이터 : kaggle의 IMDB 영화 리뷰 데이터 [🔗링크](https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
  - 데이터 전처리 
    - Label Encoder를 사용해 sentiment열의 데이터를 숫자로 인코딩 
    - 결측치, 중복값 확인 후 제거
    - 정규표현식을 이용해 영어, 숫자, 공백만 남기기 
    - 불용어 제거, 표제어 추출과 동시에 토큰화 진행 
    - Keras의 덱스트 전처리를 이용한 정수 인코딩 
    - 리뷰의 길이를 맞춰주는 패딩 진행 
    - 전처리 결과 
        
        <img width="800" alt="스크린샷 2022-02-07 오후 10 18 44" src="https://user-images.githubusercontent.com/86868063/152795482-5370a0d4-56bf-47c7-aea8-601ad49f07c4.png">
    - 모델 학습 
    
        <img width="800" alt="스크린샷 2022-02-07 오후 10 20 12" src="https://user-images.githubusercontent.com/86868063/152795683-ee09e996-f2df-4a89-9e4b-fa9a18c0286d.png">
    - 모델 선택 
        
        <img width="800" alt="스크린샷 2022-02-07 오후 10 21 49" src="https://user-images.githubusercontent.com/86868063/152795906-fce41f18-a0a7-46a5-9923-5af6755f9042.png">

       
  <br>
  
  ## 프로젝트 결과 
  - 모델 학습 결과 : Test 데이터 86% 정확도 
  - 한계점 
      - 일부 문장의 낮은 정확도 
      - 단조로운 감성 분석
      - 일부 문장의 낮은 정확도 
      - 영어 데이터 사용으로 한국어 적용 불가 
      
        <img width="800" alt="스크린샷 2022-02-07 오후 10 32 17" src="https://user-images.githubusercontent.com/86868063/152797573-706e1f48-9d5e-4cd9-82e0-2f688753a786.png">

  - 보완방안
      - 다양한 전처리 결과를 다양한 모델에 학습 한 후 비교 
      - 감성을 세분화해 다양한 감성분석 진행 
      - 한국어 데이터를 이용해 모델을 학습해 한국어에도 적용 
        
        <img width="800" alt="스크린샷 2022-02-07 오후 10 32 26" src="https://user-images.githubusercontent.com/86868063/152797798-d451d417-b6d8-4b9b-b2d2-94c616484f79.png">
        
