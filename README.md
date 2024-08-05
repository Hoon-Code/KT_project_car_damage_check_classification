# ✔️차량 파손 여부 분류 
---

## ✔️프로젝트 개요
- 주제 : 차량 공유업체의 차량 파손 여부 분류
- 학습과목 : 딥러닝, 시각지능 딥러닝
- 데이터 출처 : 자체 제작
- 유형 : classification
- 중점사항 : keras 통한 CNN모델 설계, Transfer Learning을 통한 성능 향상
---

## ✔️도메인 이해
![image](https://github.com/user-attachments/assets/3792eadb-350a-418f-8f7a-e9ee8a23984b)
![image](https://github.com/user-attachments/assets/40eca5eb-1792-4566-99eb-ec704642b449)
![image](https://github.com/user-attachments/assets/7ae5215e-cfe9-43a4-a63b-250f42658546)
![image](https://github.com/user-attachments/assets/ba965ade-8b13-42ef-8ad9-9ca0366cf0c6)
![image](https://github.com/user-attachments/assets/42855d51-9e24-4aa7-870f-6a7b3639b87c)
---

## ✔️데이터 소개
![image](https://github.com/user-attachments/assets/62c64a43-69fd-49db-b971-2dcc0481dafa)
![image](https://github.com/user-attachments/assets/a06acc4a-2cdf-4d06-92d4-5ee723d98dc9)
---

## ✔️문제 해결 프로세스
![image](https://github.com/user-attachments/assets/422102e8-3ab1-4bb7-9cab-5a7b037cb470)

## ✔️핵심사항
![image](https://github.com/user-attachments/assets/9a8729c4-7ec5-4aa0-82fc-7425f3b7438e)
---
## ✔️데이터 전처리

- 정상 차량 이미지 불러와서 이미지 및 shape 확인

![image](https://github.com/user-attachments/assets/35f8237a-468f-49e9-98f6-010c5f8306ad)

- 파손 차량 이미지 불러와서 이미지 및 shape 확인

![image](https://github.com/user-attachments/assets/b8ab78b6-c6e1-4b37-b560-bd9a1996e936)

1) 클래스 만들어서 정상 차량 이미지 와 파손 차량 이미지 만큼 라벨 만든후 합쳐주기

![image](https://github.com/user-attachments/assets/be4f5585-72fb-4724-9224-a2bf266cc0f2)

2) 전체 이미지 데이터를 하나의 리스트로 통합후 데이터 셋 분리 및 이미지를 넘파이 배열 형태로 변환

![image](https://github.com/user-attachments/assets/7814cc5a-1cc5-4a04-88c9-53658702c2cf)
![image](https://github.com/user-attachments/assets/efff51b3-98d8-40c6-a3b2-ed8b32f2c6e1)
![image](https://github.com/user-attachments/assets/4c9dd840-d28b-4cb5-a29e-b5357a128304)

## ✔️모델링 1)

![image](https://github.com/user-attachments/assets/742fc6b9-a149-45c4-b148-46997dae9e00)
![image](https://github.com/user-attachments/assets/a077504b-b00c-43be-a0c5-50a3f95c8862)

## ✔️모델링 2)

- **image_dataset_from_directory를 이용해 training set, validation set을 만들기**

![image](https://github.com/user-attachments/assets/b8ec08b8-9453-4f81-8220-c5ad49dee5fb)

- **pretrained_model인 Interception_v3를 이용해 transfer learning**
![image](https://github.com/user-attachments/assets/68fb1bf7-8835-4970-a07f-8c849a5b459c)
![image](https://github.com/user-attachments/assets/e34c9e0e-f6af-4475-92fc-2a25512fa8b9)
![image](https://github.com/user-attachments/assets/874dfbd7-9645-41fc-bb5a-781d2a80d5f1)
