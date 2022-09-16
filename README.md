<img width="700" alt="스크린샷 2022-09-16 오후 2 50 16" src="https://user-images.githubusercontent.com/97447841/190565936-59b28b3a-695c-40a2-aa24-f35e01a2cd22.png">

Date : 2022.7.11~2022.8.5

Tags : `RaspberryPi` `OpenCV` `Tensorflow` `Keras` `Python`

Link : https://github.com/heezzing/project6.git

발표영상 : [https://youtu.be/etcQFuLz-nA](https://youtu.be/etcQFuLz-nA)

시연영상 :

  - [https://youtube.com/shorts/YQ5VaTC-17k?feature=share](https://youtube.com/shorts/YQ5VaTC-17k)
  - [https://youtu.be/qjYvi7tAHwM](https://youtu.be/qjYvi7tAHwM)

## 프로젝트 내용

### 목차
<img width="700" alt="스크린샷 2022-09-16 오후 11 34 59" src="https://user-images.githubusercontent.com/97447841/190664238-9856051a-7317-44b4-8470-c6622dc9acf9.png">

------

### 프로젝트 개요
<img width="700" alt="스크린샷 2022-09-16 오후 11 56 58" src="https://user-images.githubusercontent.com/97447841/190669030-18982799-781b-4e35-91d2-4a252d350f19.png">
<img width="700" alt="스크린샷 2022-09-16 오후 11 57 11" src="https://user-images.githubusercontent.com/97447841/190669075-04f0d5fb-a51a-4529-a634-c140be6a3f23.png">

- 주제 :Raspberry Pi를 이용한 자율주행 RC CAR
- 주제 선정 이유 : 자율주행이 사고 방지에 어느 정도 역할을 수행할 수 있을지 알기 위해 주제를 선정하였습니다.
- 기대 효과 :
    - 교통사고를 예방하여 사망률을 감소 시켜줍니다.
    - 운전자의 편의성을 향상 시켜줍니다.

------

### 활용 장비 및 개발 환경
<img width="700" alt="스크린샷 2022-09-16 오후 11 58 15" src="https://user-images.githubusercontent.com/97447841/190669306-2c09a0db-e8f0-4a87-a39c-e04eda2fc681.png">

- 개발에 필요한 장비 및 환경 설정도 매우 중요합니다.
- 라즈베리 파이와 전용 RC카 모듈 키트, Pi 카메라와 RC카를 원격으로 다룰 컴퓨터 및 OS 설치용 SD카드 등이 필요합니다.
- 개발 환경에서 필요한 라이브러리마다 호환 여부를 판단하여 알맞은 버전을 선택해 설치하여 실행해야 합니다.

------

### 프로젝트 팀 구성 및 역할
<img width="700" alt="스크린샷 2022-09-16 오후 11 59 11" src="https://user-images.githubusercontent.com/97447841/190669519-36829bab-8178-494e-b7c2-b3118698da9b.png">

- 2인1팀으로 구성되어 있으며 각자 따로 역할을 두지 않고 자유롭게 소통하며 단계를 나누어 필요한 기술스택을 쌓으며 협업하는 방식으로 진행하였습니다.

------

### 프로젝트 수행 절차 및 방법
<img width="700" alt="스크린샷 2022-09-16 오후 11 59 50" src="https://user-images.githubusercontent.com/97447841/190669668-507df784-8255-4a61-8895-5ed671b8af2f.png">

1. 프로젝트 진행 방향에 대한 기획서를 작성하면서 필요한 기술 스택 여부 및 필요한 장비를 파악하여 공유 및 장비 구매를 진행하였습니다.
2. 구동에 필요한 소프트웨어 및 하드웨어 조립을 진행하였습니다.
3. OpenCV를 이용하여 차선인식을 진행하였고 RC카에 구동 테스트를 완료 후 차선 검출 테스트를 진행하였습니다.
4. cnn을 이용한 딥러닝 트레이닝을 진행하던 도중 라이브러리 충돌이 생겨 환경을 재구축하여 차선인식 주행까지 진행하였습니다.

------

### 프로젝트 구조
<img width="700" alt="스크린샷 2022-09-17 오전 12 00 29" src="https://user-images.githubusercontent.com/97447841/190669807-92e3be68-4634-4316-9902-4cd2ce068194.png">

1. 라즈베리파이에 라즈비안OS를 설치하고 기본 환경 세팅을 합니다.
2. 프로젝트에 필요한 환경 구축을 위해 파이썬, opencv등 라이브러리를 설치합니다.
3. 하드웨어 조립한 뒤 구동테스트를 합니다.
4. RC카를 구동하기 위해 adafruit , gpio 를 세팅합니다.
5. 라벨링한 데이터를 딥러닝 학습 후 차선 인식 주행을 합니다.

------

### 프로젝트 수행 결과
<img width="700" alt="스크린샷 2022-09-17 오전 12 01 38" src="https://user-images.githubusercontent.com/97447841/190670058-6c4bc1aa-4531-4c7c-95ee-7af5a2b89c54.png">

- Raspberry Pi
    - Raspbian os 64bit 설치하였습니다.
    - VNC를 이용하여 원격 환경을 조성하였습니다.
    - 파이썬은 3.9.2버전을 설치하였습니다.
    - opencv는 4.6.0버전을 설치하였습니다.
    - Tensorflow,keras 2.8.0버전을 설치하였습니다.
    - 각 라이브러리마다 호환 여부가 틀리기 때문에 환경을 재구축 하는 등 시행착오가 많았습니다.
- 하드웨어 조립
    - GPIO 라이브러리로 모터 속도를 제어하였습니다.
    - adafruit 라이브러리로 조향용 서보모터를 제어하였습니다.

<img width="700" alt="스크린샷 2022-09-17 오전 12 02 25" src="https://user-images.githubusercontent.com/97447841/190670221-f4fdc1e6-785b-4085-bd74-a1dbd3631725.png">

- 카메라를 통해 opencv라이브러리를 이용하여 기초적인 차선 인식 주행을 하였습니다.
- Lane detection Algorithms를 이용하였습니다.
- RGB인 이미지가 사용하는 색 공간은 HSV 색 공간으로 변환하고 변환된 이미지를 Canny edge detectioin으로 이미지의 가장자리를 감지합니다.
- 라인 세그먼트를 1또는 2개의 차선 라인으로 결합해 라인 기울기에 따라 좌우 차선을 감지합니다.
- 최선 좌표를 기반해 조향 각도를 찾은 뒤 감지한 차선을 따라 주행을 하며 데이터 가공을 위한 영상 데이터를 수집합니다.

<img width="700" alt="스크린샷 2022-09-17 오전 12 03 06" src="https://user-images.githubusercontent.com/97447841/190670347-6a3b63d1-b84d-4092-9cdd-741218e5e63e.png">
<img width="700" alt="스크린샷 2022-09-17 오전 12 03 19" src="https://user-images.githubusercontent.com/97447841/190670381-1348540b-5ee1-445c-93a4-481df0fb5132.png">

- 딥러닝 차선 인식 주행을 하기위해 PNG이미지와 이미지에 기록된 차선 각도를 이용하여 데이터 라벨링을 하였습니다.
- 이미지를 사용하여 정보를 정확히 파악하고 자동차의 조향 각도를 예측하기 위해 Nvidia모델을 사용하였습니다.
- Nvidia Model
    - 카메라로 입력받아 차량의 조향각도를 예측하여 출력하는 회귀모델입니다.
    - Nvidia모델에 사용된 CNN레이어는 총 30개층으로 구성되며 먼저 선과 가장자리를 추출한 뒤 마지막 신경 레이어를 통과하여 조향각도를 예측합니다.
    - 예측 각도는 주어진 이미지에서 원하는 조향각도와 비교되고 오류는 역전파를 통해 CNN훈련 프로세스로 피드백 됩니다.

------

### 시연 영상

- 시연 영상 1
    - https://youtube.com/shorts/YQ5VaTC-17k?feature=share
    
- 시연 영상 2
    - https://youtu.be/qjYvi7tAHwM

------

### 느낀점

- 처음 목표는 자율주행과 객체탐지를 접목하여 구동하는 RC카를 만드는 것 이었습니다.
- Raspberry Pi에 개발환경을 구축하는게 생각보다 힘들었고 거기에 많은 시간을 소비해서 목표한바를 이루지 못해 아쉽습니다.
- 처음부터 시간을 잘 분배했다면 완성도가 더 높았을거 같습니다.
- 이번프로젝트를 통해 자율주행에 더 흥미를 느끼게 되었고 미완성된 프로젝트를 마무리 하고 싶습니다.
