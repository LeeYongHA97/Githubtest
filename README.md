# 실습 


# Test 모델을 이용한 Test 도출

* Github Url: https://github.com/LeeYongHA97/Githubtest (꼭! 하이퍼링크)

* requirement: pandas, numpy, torch, seaborn, matplotlib

1. 수행 기관:  IMBK 데이터분석 전문가과정 (역할: Method 튜닝, 전처리, 팀장, 트러블 슈팅)

2. 데이터: 환자 데이터 10000개, 정상인 데이터 20만개

3. Method:  전처리: 이미지 Normalize + MixUp(Augmentation) + Denosing               
            모델: F-AnoGAN (Medical Image Analysis, 2019.05)
	         optimizer: Adam 
            loss: L1 loss
	<img src="https://user-images.githubusercontent.com/85111065/173891979-c4353c43-345f-4cec-8a4f-d818e00d97f5.png" width="500">

4. 결과: <br>

* Anomaly detection: <br>
	<img src="https://user-images.githubusercontent.com/85111065/173892034-27a00459-f7af-4ed7-877c-45baa59f2a10.png" width="500" >

* Acc: <br>
	<img src="https://user-images.githubusercontent.com/85111065/173892050-d0406ab4-e31b-43c1-bfa7-cd121428e1aa.png" width="500" >

* 프로젝트 수행 중 문제: 정상인 데이터에서도 미세한 Anomaly가 검출되어서, 환자로 분류하는 threshold를
    높혀줌으로써 정확히 분류될 수 있도록 조치하였으며, 데이터가 부족하여 오픈데이터를 다수 활용.

5. 참고: Schlegl, Thomas, et al. "f-AnoGAN: Fast unsupervised anomaly detection with generative 
    adversarial networks." Medical image analysis 54 (2019): 30-44.


![output](https://github.com/user-attachments/assets/567c65b4-6b2f-474d-8184-1f97015c03f5)
![architecture](https://github.com/user-attachments/assets/cf2989c2-1125-4392-b9bc-a11ac3cddf1b)














   

