# 7주차 진도보고서(정민서)
## 활동 주제
모델 선정

## 활동 내용
1. Image Segmentaion 모델 선정
   
   * Grounded-SAM
     
     -> GroundingDINO + Segment Anything(SAM)
     
     (1) GroundingDINO : 아래 사진처럼 키워드로 사물을 찾아주는 기술
     
     ![image](https://github.com/honglll111/Graduation_Project/assets/87513761/0464e304-7bb3-4e52-bc7e-7100bb559ef9)
 
     (2) Segment Anything(SAM): 사물의 바운더리를 표시해주는 기술
     
     ![image](https://github.com/honglll111/Graduation_Project/assets/87513761/781401d5-800f-4e4d-b4c3-44db496e8f2d)

     (3) Grounded-SAM: 키워드로 사물을 찾고, 바운더리 표시해주는 기술

     ![image](https://github.com/honglll111/Graduation_Project/assets/87513761/d2deb87d-5d72-4c83-9011-9e400da81579)

2. GROUNED-SAM 코드 실행
   
   https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/automated-dataset-annotation-and-evaluation-with-grounding-dino-and-sam.ipynb

   결과:
   
   ![image](https://github.com/honglll111/Graduation_Project/assets/87513761/7a10a3ee-c3b1-4d7c-966e-8217852b8f61)

   **-> DALL·E 2 그림 그려질 부분이 잘려야 하는데 이 코드에는 그런 과정이 없음(추가 예정)**

## 다음주차 계획
- Segment Anything 부분을 잘라낼 코드 추가 
