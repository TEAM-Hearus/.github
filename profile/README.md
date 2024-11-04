![image](https://github.com/user-attachments/assets/9be2766a-7aed-4c24-a1db-16652bb706fd)

</br>

Hearus는 대학교 교내 청각장애 학우 대필지원 도우미 활동에서 느낀 문제들을 풀어내기 위해 시작되었습니다. </br>
청각장애 학우들이 더 나은 환경에서 학습하고, 비장애 학우들과의 교육적 불평등을 해소할 수 있도록 하기 위해 </br>
인공지능을 활용한 실시간 음성 텍스트 변환과 문제 생성, 하이라이팅 기능을 지닌 서비스입니다.

## 주요 기능

### 1. 실시간 음성-텍스트 변환
- 강의 내용을 실시간으로 텍스트로 변환하여 자막 형태로 제공
- OpenAI Whisper 모델 활용

### 2. AI 기반 중요 단어 하이라이팅
- Ollama 및 llama3 모델이 강의 내용을 분석하여 핵심 키워드와 중요 개념을 자동으로 하이라이팅
- 학습 효율성 향상 및 복습 시간 단축

### 3. AI 맞춤형 문제 생성
- 변환된 텍스트에 기반하여 llama3 모델이 자동으로 학습 문제 생성
- 객관식, 주관식, 단답형 등 다양한 문제 유형 지원
- 문제 제공을 통해 장애 학우들에게 효과적인 학습 환경 조성

### 4. 시간표 형식의 스크립트 관리
- 변환된 강의 스크립트를 시간표 형식으로 직관적으로 관리
- 강의별, 날짜별 쉬운 검색 및 접근 기능

## 🛠 프로젝트 아키텍처
![image](https://github.com/user-attachments/assets/25b93d80-f06d-4486-8da0-6724bc4b7d32)

### Frontend: React
- 최신 React Hooks 및 상태 관리 라이브러리 활용
- 아토믹(atomic) 디자인 시스템 차용
- 커스텀 404 Not Found 페이지 구현

### Backend: Spring
- Spring Boot 기반의 확장 가능한 아키텍처
- RESTful API 설계 및 구현
- 보안 및 인증 시스템 통합
- 실시간 음성인식을 위한 WebSocket, Socketio 기반 서버 구축

### AI Serving: FastAPI
- 고성능 비동기 처리를 위한 FastAPI 프레임워크 사용
- 실시간 음성 인식 및 자연어 처리 모델 서빙
- API 기반 LLM 및 AI Model 서빙 LangChain 구축

### Infrastructure: AWS
- 고가용성 및 확장성을 위한 클라우드 네이티브 아키텍처
- 컨테이너화된 마이크로서비스 배포 (ECS, EBS, Spot Instance)
- 서버리스 컴퓨팅 활용 (Lambda, Step Function, EventBridge)
- GPT API가 아닌 자체 AI Serving 서버 구현 및 인스턴스 구축

<!--
## 📊 프로젝트 현황

![GitHub stars](https://img.shields.io/github/stars/TEAM-Hearus/HEARUS-REACT-FRONTEND?style=social)
![GitHub forks](https://img.shields.io/github/forks/TEAM-Hearus/HEARUS-REACT-FRONTEND?style=social)
![GitHub pull requests](https://img.shields.io/github/issues-pr/TEAM-Hearus/HEARUS-REACT-FRONTEND)
</br>
![GitHub stars](https://img.shields.io/github/stars/TEAM-Hearus/HEARUS-SPRING-BACKEND?style=social)
![GitHub forks](https://img.shields.io/github/forks/TEAM-Hearus/HEARUS-SPRING-BACKEND?style=social)
![GitHub pull requests](https://img.shields.io/github/issues-pr/TEAM-Hearus/HEARUS-SPRING-BACKEND)
</br>
![GitHub stars](https://img.shields.io/github/stars/TEAM-Hearus/HEARUS-AI-SERVING?style=social)
![GitHub forks](https://img.shields.io/github/forks/TEAM-Hearus/HEARUS-AI-SERVING?style=social)
![GitHub pull requests](https://img.shields.io/github/issues-pr/TEAM-Hearus/HEARUS-AI-SERVING)

-->
---

<p align="center">
  모두의 들을 권리를 위하여 Hearus가 함께하겠습니다
  </br></br>
  <img src="https://img.shields.io/badge/TEAM-Hearus-FF603D?style=for-the-badge" alt="TEAM-Hearus">
</p>
