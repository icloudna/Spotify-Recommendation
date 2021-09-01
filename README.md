# Spotify-Recommendation
<img src="https://user-images.githubusercontent.com/87663692/130558207-ea001f58-20e6-46a5-a230-8f87d44503df.png" width="550" height="300"/>

## 프로젝트 소개 (2021.03.11 ~ 2021.04.06)
다양한 추천 시스템 이론을 학습하고, Spotify의 추천시스템을 구현하는 것을 목적으로 합니다.
이에 추천시스템 스터디를 함께 진행하며 실습 경험을 위주로 진행하였습니다.

정기 세션: 화요일 밤 10시 30분~
- 2021.03.11(목) : 정기 일정 및 계획 설정
- 2021.03.16(화): 데이터 전처리 완료, Classifier 선택
- 2021.03.23(화): Classifier 성능 확인
- 2021.03.30(화): Recommender System 모델 학습 및 선정
- 2021.04.06(화) : 최종점검

## 팀원 소개
김도윤, 김창현, 기다연, 임효진, 이나윤

## 교재 소개
Python을 이용한 개인화 추천시스템(도서출판청람)
모든 단원을 공부하며, Surprise의 다양한 추천 시스템을 구현해보았습니다.
<img src="https://user-images.githubusercontent.com/87663692/130485877-714a4312-af90-48fe-abfa-baa3438caff4.png" width="200" height="250"/>
                                                                                                                   
## 데이터 소개
- 각 노래의 특징을 담은 Dataset (Track_Features.csv)
: Acousticness, Danceability, Duration_ms, Energy, Instrumentalness, Key, Liveness, loudness, mode, speechiness, tempo, time_signiture, valence

- 각 노래에 수동으로 라벨링한 Dataset (Ratings.csv)
: 긍정(1), 모름(0), 부정(-1) 부여하여 총 29명의 data 확보.
 
- 각 노래에 수동으로 라벨링한 User에 대한 부가적인 Dataset (User.csv)
: gender(M/W), age, nationality 

## 개인적으로 맡았던 Modeling
- Classification (한 사용자의 음악 트랙에 대한 선호 유무 분류): Lasso, Ridge, Elastic Net

- Recommendation: Coclustering(Surprise)

## Conclusion
- 추천시스템 모델의 경우, 사용자 수가 더 많고 음악 트랙이 다양했더라면 더 일반적인 좋은 성능을 얻었을 것 같다.
(개인적으로, 이미 시중에 있는 데이터를 활용하다보니 사람들에게 더 익숙한 최신 노래보다는 시간이 좀 지난 팝송에 데이터가 치중되어 아쉬웠음.)

- User, Track_Features의 추가 활용 방안이 필요하다.
(이번 프로젝트에서는 Item-based Recommendation 모델을 구현했기 때문에, User-based 특징도 띄는 모델도 만들어보면 좋을 것 같다.)
(또한, Track_Features 추천시스템이 음악을 구분하는 기준으로만 사용했는데, 이 외에도 이를 활용할 수 있는 방법이 있을까 고민이 되었다.)
