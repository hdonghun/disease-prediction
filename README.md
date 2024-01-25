<h2>
<div align="center"># 비대면 진료 음성 인식 및 텍스터 분석 서비스 프로젝트 </div>
  <h4> 자연어 인식 프로젝트 </h4>
</h2>

<h3>✨서비스 소개</h3>

### 비대면 진료 희망하는 사람 + 진료에 대한 인프라가 부족한 곳에 있으신 분들(해외나 시골에 있어서) 위한 비대면 진료 서비스(임시 제목입니다)

1. **문제 정의 및 목표 설정**:
    - 서비스 기획의 첫 번째 단계는 어떤 문제를 해결하고자 하는지 명확하게 정의하는 것입니다. → 해외 거주하는 재외동포들의 효율적이고/편리한 진료 서비스를 위해서
    - 딥러닝을 통해 해결하고자 하는 문제와 목표를 설정합니다. 예를 들어, 이미지 분류, 자연어 처리, 추천 시스템 등 다양한 문제에 딥러닝을 적용할 수 있습니다.
        
        → 환자/간호사/의사의 음성 데이터들을 전처리 후 모델에 학습 시켜, 환자 상태에 대한 간단한 분석 및 치료방법(추천 시스템 구축)
        
2. **데이터 수집 및 전처리**:
    - 딥러닝 모델을 학습시키기 위한 데이터를 수집하고 전처리합니다. 이 단계에서 데이터의 품질을 검토하고 필요한 경우 데이터를 정제하거나 가공합니다.
        
        → 음성데이터를 STT기법을 통해, 텍스트화하고, 불필요한 불용어 제거 및 커스텀화
        
    - 라벨링된 데이터를 얻는 것이 중요하며, 데이터 양과 품질은 모델 성능에 큰 영향을 미칩니다. → 이 부분에 대해서는, 기존 데이터셋에 라벨링된 데이터가 존재한다.
3. **모델 선택 및 설계**:
    - 문제에 맞는 딥러닝 모델을 선택하고 설계합니다. 모델의 아키텍처, 레이어, 하이퍼파라미터 등을 결정합니다. → 각자 많은 모델을 사용 함으로써, 최적의 모델을 선택하여 공유
    - 모델의 복잡성과 성능을 고려하여 최적의 모델을 선택합니다.
        
        → 여러가지 모델이 있기 때문에, 각자 조사하여 사용 해보고, 공유하면 좋을 꺼 같습니다!
        
4. **모델 학습 및 검증**:
    - 선정한 모델을 학습시키고 검증합니다. 학습 데이터를 사용하여 모델을 학습하고, 검증 데이터를 사용하여 모델의 성능을 평가합니다.
        
        → 이 부분에서 대회 규칙인, 성능지표를 기반
        
        - **제1 평가지표 : CER(Character Error Rate)**
            - Substitution (*S*): 추론된 텍스트 중 정답 텍스트와 비교해 잘못 대체된 음절 수
            - Deletion (*D*): 추론된 텍스트 중 정답 텍스트와 비교해 잘못 삭제된 음절 수
            - Insertion (*I*): 추론된 텍스트 중 정답 텍스트와 비교해 잘못 추가된 음절 수
            - *N*: 정답 텍스트의 음절 수
        - **제2 평가지표 : WER(Word Error Rate)**
            
             - Substitution (*S*): 추론된 텍스트 중 정답 텍스트와 비교해 잘못 대체된 단어 수
            
             - Deletion (*D*): 추론된 텍스트 중 정답 텍스트와 비교해 잘못 삭제된 단어 수
            
             - Insertion (*I*): 추론된 텍스트 중 정답 텍스트와 비교해 잘못 추가된 단어 수
            
             - *N*: 정답 텍스트의 단어 수
            
    - 오버피팅(Overfitting)을 방지하기 위한 정규화 기법을 적용하고, 하이퍼파라미터를 조정하여 최적의 성능을 얻습니다.
        
        → 평가 지표의 성능을 높이기 위해, 각자 하이퍼파라미터를 조정, 최적의 성능을 얻기 위해 노력!
        
5. **서비스 통합 및 배포**:
    - 학습된 딥러닝 모델을 실제 서비스에 통합하고 배포합니다. 이 단계에서는 모델을 서버 또는 클라우드 환경에 배포하고, API 형태로 서비스와 연결합니다.
        
        → 이 부분에 대해서, 파이널 프로젝트 할 떄, 꼭 필요한 부분이기 때문에, 여유/시간이 있다면 꼭 같이 해보면 좋을 꺼 같습니다. 
        
6. **성능 모니터링 및 향상**:
    - 서비스가 운영되는 동안 모델의 성능을 지속적으로 모니터링하고, 필요한 경우 모델을 개선합니다.
        
        → PPT발표 할 떄, 필요
        
    - 새로운 데이터나 사용자 피드백을 기반으로 모델을 업데이트하고 향상시킵니다.
        
        → PPT 발표 할 때, 필요
        
7. **윤리 및 보안 고려**:
    - 사용자 데이터의 개인정보 보호와 모델의 공정성을 고려해야 합니다. 데이터 수집 및 모델 학습 시 윤리적인 측면을 고려하고 보안을 강화해야 합니다.
        
        → PPT 발표 할 때, 이러한 부분을 간단하게 같이 설명하면 좋을 꺼 같습니다.
        
8. **마케팅 및 사용자 교육**:
    - 서비스를 성공적으로 런칭하기 위해 마케팅 전략을 수립하고 사용자에게 서비스를 소개하고 교육하는 것이 중요합니다.
        
        →  PPT 발표 할 때, 서비스적 측면에서 간단한 설명을 할 수 있으면 좋을 꺼 같습니다.
        
9. **피드백 수집 및 개선**:
    - 서비스를 사용하는 사용자로부터 피드백을 수집하고, 이를 토대로 서비스를 개선합니다. 사용자 요구사항에 맞게 지속적으로 발전시켜야 합니다.
        
        → PPT 발표 할 때, 필요

<h3>✨노션</<h3>
NOTION - https://www.notion.so/6d42ba35c01243348ed9a3a9be9b6e0a


<h3>✨기술 스택</h3>

<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"><img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">

<h3>✨툴</h3>

<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white"><img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white"><img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white"><img src="https://img.shields.io/badge/jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white">


<h3>✨프로젝트 PPT</<h3>
<details>
<summary>PPT</summary>
<img width="1580" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/ecb0ccad-c26c-43db-9358-40555df7d91b">
<img width="1577" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/f208ecdd-fdfa-4273-9166-8006f43e17ed">
<img width="1577" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/04368a33-de68-4b4a-b655-f66ae55b70d1">
<img width="1576" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/4d0d7ae0-8779-40f8-98a7-d96e1493a61a">
<img width="1578" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/4ee701ea-e1de-4a8c-bfc8-6fe8fc372fe3">
<img width="1578" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/a31b20d2-b831-4a7d-91de-8a2c65e514b7">
<img width="1574" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/fe0ec58e-1788-4325-a984-3cd0e6ba259d">
<img width="1576" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/7d858112-ad06-4b62-ba90-b309cb686db9">
<img width="1578" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/61146890-211c-4325-8e04-4f42eb5ff886">
<img width="1577" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/1e67e15e-ae31-4a52-872e-cc1d5b14c72e">
<img width="1576" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/17e80cf8-35a4-46e9-9f6a-e439320ce405">
<img width="1579" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/63c94a35-7be4-4059-8daa-3139a5387a79">
<img width="1577" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/365caf40-3a81-4204-95bf-8ae4052ab6dd">
<img width="1577" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/9207e257-9d9f-4ac8-9ab3-603f14aa7858">
<img width="1579" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/2cc17cf8-c2d7-4e7f-ac6f-9d1bcb58d2ba">
<img width="1575" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/63ccd7df-cbb9-4880-b4a1-b9af54c445af">
<img width="1577" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/ed891b12-3acd-4fa4-b69b-1bd6720399d3">
<img width="1579" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/a57cbffe-df74-47e0-96b6-8818740e5739">
<img width="1576" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/1c323517-58a0-474c-9d29-c4ba8ee00ce6">
<img width="1579" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/6647fdda-d883-4942-8e00-05ba9c446958">
<시연 영상> https://github.com/hdonghun/disease-prediction/assets/67058000/da3aea67-5e0d-44d0-b323-b0bb49315385
<img width="1580" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/d6279ee8-94a7-42b1-aecb-5f2cedb339a4">
<img width="1577" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/e08eaecf-d99d-4564-9d0a-18050075fbe4">
<img width="1579" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/9bd44c32-e831-4671-bc3b-f91beaba7068">
<img width="1574" alt="image" src="https://github.com/hdonghun/disease-prediction/assets/67058000/8d1fa27b-6157-4acb-be3e-85f87a54cb9a">






