# Hearus

<img width="1144" alt="image" src="https://github.com/user-attachments/assets/34d51edf-05d5-4199-9373-547510c51540">
</br>
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

히어러스는 대학교 교내 청각장애 학우 대필지원 도우미 활동에서 느낀 문제들을 풀어내기 위해 시작되었습니다. </br>
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

### 5. 장애 학우 접근성 강화 UI/UX
- 장애인을 위한 UI/UX 가이드라인을 준수한 인터페이스 설계
- 직관적인 내비게이션 및 명확한 아이콘 사용으로 사용성 개선
- 스크린 리더 호환성 및 키보드 네비게이션 지원

## 🛠 기술 스택
![image](https://github.com/user-attachments/assets/25b93d80-f06d-4486-8da0-6724bc4b7d32)

### Frontend: React
- 최신 React Hooks 및 상태 관리 라이브러리 활용
- 반응형 디자인으로 다양한 디바이스 지원
- 웹 접근성 표준 (WCAG 2.1) 준수

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

## 📁 Repository 구조

- [HEARUS-REACT-FRONTEND](https://github.com/TEAM-Hearus/HEARUS-REACT-FRONTEND): React 기반 웹 애플리케이션
- [HEARUS-SPRING-BACKEND](https://github.com/TEAM-Hearus/HEARUS-SPRING-BACKEND): Spring Boot 기반 API, Socket 서버
- [HEARUS-AI-SERVING](https://github.com/TEAM-Hearus/HEARUS-AI-SERVING): FastAPI 기반 AI 모델 서빙

각 Repository에는 상세한 설정, 실행 방법, 그리고 기여 가이드라인이 포함되어 있습니다.

## 🚀 시작하기

1. 각 Repository를 클론합니다:
2. 각 README의 지침에 따라 개발 환경을 설정합니다.
3. 전체 시스템을 로컬에서 실행하거나 AWS 환경에 배포합니다.

자세한 설정 및 배포 방법은 각 Repository의 README를 참조해 주세요.

## 🤝 기여하기

Hearus의 발전에 기여해 주셔서 감사합니다! 우리는 모든 형태의 기여를 환영합니다.

1. 이슈 생성: 버그 리포트, 기능 제안, 또는 질문
2. 풀 리퀘스트: 코드 개선, 문서화, 또는 새로운 기능 구현
3. 코드 리뷰: 다른 기여자의 PR을 리뷰하고 피드백 제공
4. 문서화: README, 위키, 또는 코드 주석 개선

자세한 기여 가이드라인은 [CONTRIBUTING.md](CONTRIBUTING.md)를 참조해 주세요.

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 이는 여러분이 이 소프트웨어를 자유롭게 사용, 수정, 배포할 수 있음을 의미합니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

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

## 🙏 감사의 말

이 프로젝트는 다음과 같은 오픈소스 프로젝트들의 도움을 받아 제작되었습니다:

- 🔵 [React](https://reactjs.org/) - 사용자 인터페이스 구축
- 🍃 [Spring Boot](https://spring.io/projects/spring-boot) - 백엔드 서버 개발
- ⚡ [FastAPI](https://fastapi.tiangolo.com/) - AI 모델 서빙
- 🧠 [TensorFlow](https://www.tensorflow.org/) - 머신러닝 모델 개발 및 훈련
- 🔥 [PyTorch](https://pytorch.org/) - 딥러닝 모델 개발 및 훈련
- 🎬 [FFmpeg](https://ffmpeg.org/) - 멀티미디어 처리
- 🗣️ [Whisper](https://github.com/openai/whisper) - 음성 인식 모델
- 🦙 [Ollama](https://ollama.ai/) - 로컬 LLM 실행 및 관리
- 🌐 [WebSocket](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) - 실시간 양방향 통신
- 🔌 [Socket.IO](https://socket.io/) - 실시간 이벤트 기반 통신

그리고 무엇보다 이 프로젝트에 관심을 가져주시고 지원해 주신 모든 분들께 깊은 감사를 드립니다.

</br>

---

<p align="center">
모두의 들을 권리를 위하여 Hearus가 함께하겠습니다
</p>
