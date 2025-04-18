# ML_HIIT
Machine Learning Team Project - Human Activity Recognition

This project is based on <a href="https://knu-p4c-lab.github.io/lectures/bb2bca2d-537e-5332-82b1-cf8f07ca885b/" target="_blank">**'2024 Spring Machine Learning(2)'**</a> by KNU P4C Lab.

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white"> <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white"> <img src="https://img.shields.io/badge/ScikitLearn-F7931E?style=for-the-badge&logo=ScikitLearn&logoColor=white"> <img src="https://img.shields.io/badge/Tensorflow-FF6F00?style=for-the-badge&logo=Tensorflow&logoColor=white"> <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=Keras&logoColor=white"> 

### Team Information
- Team Name : 휴먼 러닝
- Members : 이정민, 이정훈, 조성혁
- <a href="https://github.com/users/liebenholz/projects/2" target="_blank">Team Project Github Link</a>

## 1. Sensor Data Collection for HIIT Workout

프로젝트의 목적은 스마트폰의 가속도계Accelerometer 및 각속도계Gyroscope로부터 수집된 센서 데이터를 활용, HIIT 운동 프로그램의 각 운동들을 실시간으로 분류하는 기계 학습 모델을 훈련하는 것.

본 첫 번째 팀 과제에서는 기계 학습 모델 구축을 위한 사전 단계로 실제 HIIT 운동 프로그램을 수행하면서 센서 데이터를 수집함.

### HIIT

고강도 인터벌 트레이닝High-Intensity Interval Training으로, 고강도의 운동과 휴식을 번갈아가면서 하는 훈련 프로그램. 짧은 시간내에 많은 양의 칼로리를 소모할 수 있어서 체중 감량에 효과적인 것으로 알려져있음. [YouTube](https://www.youtube.com/watch?v=-hSma-BRzoo)

자세한 내용은 [설명 문서](https://docs.google.com/document/d/1lphQPFxZrGUJ2EBI5urmJG3JM_YP6eW_2CEfZHDD0cU/edit?tab=t.0)를 참고.

### Result
`team1` 폴더에서 각 인원의 데이터 수집 결과가 excel 파일을 확인 가능.

[운동별 데이터 시각화](https://github.com/liebenholz/ML_HIIT/blob/main/team01/graph_check.ipynb) 자료를 통해 센서의 계형 확인.


## 2. Model Building and Evaluation for HAR

<a href="https://www.kaggle.com/competitions/2024-knu-ml-team-asmt" target="_blank">Kaggle Competition</a>에 참여해 학생들이 직접 수집한 HIIT Workout 데이터를 활용해 9종의 행동을 인식하는 기계 학습 모델을 훈련.

`train_accel.csv` `test_accel.csv`는 가속도계 데이터, `train_gyro.csv` `test_gyro.csv`는 각속도계 데이터를 담고 있으며, `train_label.csv`는 학생의 id와 workout 값을 담고 있음. 1~8은 각각의 운동, 0은 휴식을 의미함.


`sample_submission.csv`는 train data를 기반으로 test data의 값들을 예측한 결과를 제출하는 양식임.

### Result

`team2` 폴더에서 주요 데이터 분석 및 기계학습 모델 학습 코드를 확인 가능. 

Balanced Accuracy: public: 0.79173, **private: 0.79353**

