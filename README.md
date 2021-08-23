# Spotify-Recommendation
<img src="https://user-images.githubusercontent.com/87663692/130484599-9fce212a-1d93-4ff3-b243-c313d96dfe9b.png" width="600" height="400"/>


## 프로젝트 소개 (2021.03.11 ~ 2021.04.06)
다양한 추천 시스템 이론을 학습하고, Spotify의 추천시스템을 구현하는 것을 목적으로 합니다.
이에 추천시스템 스터디를 함께 진행하며 실습 경험을 위주로 진행하였습니다.
<img src="https://user-images.githubusercontent.com/87663692/130482467-f7d26e57-2abe-4f6d-9783-3eef171b85a5.png" width="600" height="400"/>

## 팀원 소개
김도윤, 김창현, 기다연, 임효진, 이나윤

## 교재 소개
Python을 이용한 개인화 추천시스템(도서출판청람)
<img src="https://user-images.githubusercontent.com/87663692/130485877-714a4312-af90-48fe-abfa-baa3438caff4.png" width="300" height="400"/>
                                                                                                                   
## 데이터 소개
- 각 노래의 특징을 담은 Dataset (Track_Features.csv)
: Acousticness, Danceability, Duration_ms, Energy, Instrumentalness, Key, Liveness, loudness, mode, speechiness, tempo, time_signiture, valence

- 각 노래에 수동으로 라벨링한 Dataset (Ratings.csv)
: 긍정(1), 모름(0), 부정(-1) 부여하여 총 29명의 data 확보.
 
- 각 노래에 수동으로 라벨링한 User에 대한 부가적인 Dataset (User.csv)
: gender(M/W), age, nationality 

## 개인적으로 맡았던 Modeling
- Classification (한 사용자의 음악 트랙에 대한 선호 유무 분류): Lasso, Ridge, Elastic Net

- Recommendation: Coclustering

## Conclusion
- 추천시스템 모델의 경우, 사용자 수가 더 많고 음악 트랙이 다양했더라면 더 일반적인 좋은 성능을 얻었을 것 같습니다.
- User, Track_Features의 추가 활용 방안이 필요합니다.
(이번 프로젝트에서는 Item-based Recommendation 모델을 구현했기 때문에, User-based 특징도 띄는 모델도 만들어보면 좋을 것 같습니다.)

