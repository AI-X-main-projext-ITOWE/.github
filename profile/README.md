## ITOWE's Project

![header](https://capsule-render.vercel.app/api?type=waving&color=2E64FE&height=250&section=header&text=%20💪fitchecker&fontSize=50&animation=twinkling&fontColor=FFFF00&desc=ItoWe🤸‍♂️&stroke=FFFFFF&strokeWidth=3&rotate=-20&fontAlign=50&fontAlignY=50)

## ![christmas-tree (1)](https://github.com/user-attachments/assets/8d99d631-42de-44c5-9505-760b92f7f4ab) FitChecker - AI로 운동 자세 교정과 최신 정보를 제공하는 맞춤형 운동·식단 솔루션.

FitChecker는 AI 기반 운동 자세 교정 및 개인 맞춤형 운동과 식단 추천을 통해 체계적이고 효과적인 건강 관리와 운동 성과를 돕는 혁신적인 AI 솔루션입니다. 카메라와 AI 기술을 활용해 올바른 자세를 유도하고, AI 챗봇을 통해 개인별 최적의 운동과 식단 정보를 제공합니다.

- **운동 자세 감지 및 교정**  : 잘못된 자세를 감지하고 즉각적인 교정 피드백을 제공합니다.

- **AI 챗봇을 통한 맞춤형 정보 제공**  : 개인별 상태와 목표에 맞춘 최적의 운동 계획과 식단을 추천합니다.

- **개인 맞춤형 운동 및 식단 솔루션**  : 사용자의 건강 상태와 목표를 분석해 AI가 가장 효과적인 맞춤형 운동과 식단을 제공합니다.  

<br>

##  ![beanie (1)](https://github.com/user-attachments/assets/99fcfa73-8024-4c82-bd43-31dfffc27a91) Features

1. **운동 자세 감지 및 교정**  
   - **MediaPipe Pose**: 33개의 신체 관절 포인트를 감지하여 정확한 자세 추출  
   - **CameraX**: 실시간 카메라 프레임 처리로 저지연 자세 감지 제공  
   - 잘못된 자세 감지 시 **시각적 및 음성 피드백**으로 교정 유도  

2. **AI 챗봇을 통한 맞춤형 정보 제공**  
   - **Elasticsearch**: 대규모 운동 및 식단 데이터 인덱싱과 빠른 검색  
   - **RAG (Retrieval-Augmented Generation)**: 최신 데이터와 AI를 결합해 정확하고 전문화된 정보 제공  
   - AI 챗봇이 **자연어 처리**를 통해 사용자의 요청을 이해하고 적절한 피드백 제공  

3. **Agent 기능: 스마트 운동 관리**  
   - **스케줄러**: 운동 시간, 세트, 반복 횟수 알림 설정 및 관리  
     - 예: "스쿼트 3세트 2회, 오후 3시 30분 알림"  
   - **자동 화면 전환**: 운동 요청 시 실시간 자세 감지 화면 자동 실행  
     - 예: "풀업 3세트 2회 시작할게" → **자세 감지 화면 활성화**  

4. **개인 맞춤형 솔루션**  
   - 사용자 건강 데이터를 기반으로 **운동 및 식단 추천 알고리즘** 제공  
   - 데이터 분석과 지속적인 피드백을 통해 맞춤형 운동 및 식단 솔루션 최적화  

5. **Firebase 통합**  
   - **Firebase Authentication**: 사용자 로그인 및 인증 관리  
   - **Firebase Firestore**: 사용자 데이터(운동 이력, 목표, 스케줄 등) 저장 및 관리  
   - **Firebase Cloud Messaging**: 운동 알림 및 식단 스케줄 푸시 알림 전송  
   - **Firebase Hosting**: 앱 배포 및 호스팅을 통한 안정적 서비스 제공  

6. **데이터 관리 및 확장성**  
   - **Elasticsearch 클러스터**를 통한 확장 가능한 데이터 관리  
   - **Firebase**와 **Elasticsearch**의 연동으로 빠르고 안정적인 데이터 접근 및 처리  
   - **API 기반 아키텍처**: 클라이언트-서버 간 효율적인 데이터 통신 및 관리  
<br>

##  ![christmas-wreath](https://github.com/user-attachments/assets/14b16910-895e-4fcc-889d-884ca572b5c2) Branch
<br>

이 프로젝트는 효율적인 협업과 안정적인 배포를 위해 `release`, `dev`, `feature` 브랜치를 사용하는 Git 브랜치 전략을 채택했습니다.
![깃허브 전략](https://github.com/user-attachments/assets/2625e974-353b-4db6-bb78-7fe33258ecfc)


### 🔹 `feature` Branch
- **목적**: 새로운 기능이나 버그 수정을 개발하는 브랜치입니다.
- **사용 방법**: 각 기능 또는 수정 사항마다 별도의 `feature` 브랜치를 생성하며, 브랜치 이름은 `feature/기능명` 형식을 따릅니다.

### 🔹 `dev` Branch
- **목적**: 통합 개발을 위한 브랜치로, 모든 `feature` 브랜치의 변경 사항이 이곳에서 모여 테스트됩니다.
- **사용 방법**: 기능별 개발이 완료되면 `dev` 브랜치에서 전체적으로 테스트하고 오류를 확인합니다.

### 🔹 `release` Branch
- **목적**: 배포 준비가 완료된 안정적인 코드를 관리하는 브랜치입니다.
- **사용 방법**: `dev` 브랜치에서 충분한 테스트가 완료된 후 `release` 브랜치로 이동하여 실제 배포를 진행합니다.

이 브랜치 전략을 통해 기능 개발부터 배포까지 안정적으로 관리하며, 코드의 품질을 유지하고 있습니다.

<br>

## ❄ STACK

![image](https://github.com/AI-X-main-projext-ITOWE/.github/blob/main/stack.png)


<br>

##  ![christmas-gloves](https://github.com/user-attachments/assets/b4690dad-108c-4d8b-bfee-e4be5db3a854) Architecture



<br>


## ⛄ Contributor

+ hwangjeonghan | 황정한 | [깃허브](https://github.com/hwangjeonghan)

+ Shineunhan | 신은한 | [깃허브](https://github.com/Shineunhan)

+ parkkkkjuneHyeon | 박준현 | [깃허브](https://github.com/parkkkkjuneHyeon)

+ jinnyjinny12 | 서은진 | [깃허브](https://github.com/jinnyjinny12)

+ Jin-tonix | 목진희 | [깃허브](https://github.com/Jin-tonix)

+ oct1H | 최상훈 | [깃허브](https://github.com/oct1H)


<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
