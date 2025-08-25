# 🚀 LV.0 - LLM Vulnerability Zero

<div align="center">

<img width="646" height="344" alt="1_JFZE1HIpXk9e16Jg53cNzg" src="https://github.com/user-attachments/assets/1806ffb2-a28d-4a02-849c-47786555dd37" />


**AI 기반 코드 보안 취약점 자동 분석 및 리포팅 플랫폼**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![React](https://img.shields.io/badge/React-18+-61dafb.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-3178c6.svg)](https://www.typescriptlang.org/)

</div>

## 📖 개요

LV.0 (LLM Vulnerability Zero)는 **AI 기반의 오픈소스 보안 취약점 자동 분석 및 리포팅 도구**입니다. 사용자가 소스 코드 프로젝트를 업로드하면, 정적 분석과 LLM(Claude)을 통해 취약점을 탐지, 분석하고 상세한 PDF 리포트를 생성합니다.

### ✨ 주요 기능

- 🔍 **정적 코드 분석**: Semgrep을 활용한 다국어 보안 취약점 탐지
- 🤖 **AI 기반 분석**: Anthropic Claude를 통한 지능형 취약점 분석
- 📊 **상세한 리포트**: PDF 형태의 전문적인 보안 분석 보고서
- 🚀 **실시간 처리**: 비동기 처리로 대용량 프로젝트 지원
- 🌐 **웹 인터페이스**: React + TypeScript 기반의 현대적인 UI

## 🏗️ 아키텍처
<img width="9049" height="4151" alt="LV 0 System Architecture (2)" src="https://github.com/user-attachments/assets/9606ba68-4811-441a-8b87-4bb4329349bd" />

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │    │   Flask-A       │    │   Flask-B       │
│   (React/TS)    │◄──►│   (Static       │◄──►│   (LLM/Report)  │
│   Port: 5173    │    │    Analysis)    │    │   Port: 5001    │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                                │                       │
                                ▼                       ▼
                       ┌─────────────────┐    ┌─────────────────┐
                       │   Analysis      │    │   Workspace     │
                       │   Engine        │    │   Management    │
                       │   (Semgrep)     │    │   (File I/O)    │
                       └─────────────────┘    └─────────────────┘
```

## 🛠️ 기술 스택

### Frontend
- **React 18** - 사용자 인터페이스
- **TypeScript** - 타입 안전성
- **Vite** - 빠른 개발 및 빌드
- **Electron** - 데스크톱 앱 지원
<img width="1584" height="992" alt="1" src="https://github.com/user-attachments/assets/24da1b4d-2ae0-4089-a0a4-c0aef461be37" />
<img width="1584" height="992" alt="2" src="https://github.com/user-attachments/assets/b4d40bd7-685f-473f-a7b0-4d33c0e5a493" />
<img width="1585" height="992" alt="3" src="https://github.com/user-attachments/assets/4ef3b0a5-4d95-4e43-9364-5c288c4b35ac" />
<img width="1585" height="992" alt="4" src="https://github.com/user-attachments/assets/28ebbef3-887b-4a22-8c8d-f0c39c0fdc58" />
<img width="1585" height="992" alt="5" src="https://github.com/user-attachments/assets/a8a28e12-fcbe-43ff-904d-b549c8ed21af" />
<img width="1585" height="992" alt="6" src="https://github.com/user-attachments/assets/e717ecef-194c-4e50-b61a-a7a413de13d5" />

### Backend
- **Flask** - 마이크로서비스
- **Python 3.8+** - 백엔드 로직

### Security & Analysis
- **Semgrep** - 정적 코드 분석
- **Anthropic Claude** - AI 기반 취약점 분석

## 프로젝트 구조

```
LV.0-LLM-Vulnerability-Zero/
├── 📁 frontend/                 # React 프론트엔드
│   ├── 📁 src/
│   │   ├── 📁 pages/           # 페이지 컴포넌트
│   │   ├── 📁 services/        # API 서비스
│   │   └── 📁 assets/          # 이미지 및 리소스
│   ├── 📁 electron/            # Electron 설정
│   ├── 📁 dist/                # 빌드 결과물
│   ├── 📄 package.json         # Node.js 의존성
│   ├── 📄 vite.config.ts       # Vite 설정
│   └── 📄 tsconfig.json        # TypeScript 설정
├── 📁 flask-a/                  # 정적 분석 서비스
│   ├── 📁 analysis/            # 분석 엔진
│   ├── 📁 uploads/             # 업로드된 파일
│   ├── 📁 outputs/             # 분석 결과
│   ├── 📁 final_output/        # 최종 출력
│   ├── 📄 app.py               # Flask 애플리케이션
│   ├── 📄 forwarder.py         # 요청 전달 로직
│   └── 📄 requirements.txt     # Python 의존성
├── 📁 flask-b/                  # LLM 분석 서비스
│   ├── 📁 workspace/           # 작업 공간
│   ├── 📁 received/            # 수신된 파일
│   ├── 📄 analyzer.py          # LLM 분석 로직
│   ├── 📄 llm_utils.py         # Claude API 연동
│   ├── 📄 utils.py             # 유틸리티 함수
│   ├── 📄 unzipper.py          # 압축 해제 로직
│   └── 📄 requirements.txt     # Python 의존성
├── 📄 .gitignore               # Git 제외 파일
├── 📄 package.json             # 루트 패키지 설정
└── 📄 README.md                # 프로젝트 문서
```

## 🚀 빠른 시작

### 1. 사전 요구사항

- **Python 3.8+**
- **Node.js 18+**
- **Anthropic API 키** (Claude 사용)

### 2. 저장소 클론

```bash
git clone https://github.com/Gaurdians-of-the-Open-Source/final-result.git
cd final-result
```

### 3. 환경 변수 설정

프로젝트 루트에 `.env` 파일을 생성하고 다음 내용을 추가하세요:

```bash
# Anthropic Claude API 키 (필수)
ANTHROPIC_API_KEY=sk-ant-api03-your-actual-key-here
```

### 4. 백엔드 서비스 실행

```bash
# Flask-A 실행 (정적 분석 서비스)
cd flask-a
pip install -r requirements.txt
python app.py

# Flask-B 실행 (LLM 분석 서비스) - 새 터미널에서
cd flask-b
pip install -r requirements.txt
$env:ANTHROPIC_API_KEY="your_anthropic_api_key_here" (환경변수 설정)
python app.py
```

### 5. 프론트엔드 실행

```bash
# 프론트엔드 실행
cd frontend
npm install
npm run dev
```

### 6. 접속

- **프론트엔드**: http://localhost:5173
- **Flask-A**: http://localhost:5000
- **Flask-B**: http://localhost:5001

## 💻 사용 방법

### 1. 사용 방법 소개

1. **Flask-A와 Flask-B의 app.py를 각각 실행**합니다. (Flask-B를 실행시킬 때에는 자신의 Claude Sonnet 4 버전의 API를 환경변수로 지정하여 실행합니다)
2. **cd frontend**를 하여 frontend에서 **npm run dev**를 통해 프론트엔드를 실행시킵니다.
3. **Get Started**를 누르고 다음 페이지로 넘어가지면 **Start Analysis**를 눌러서 취약점 분석을 시작합니다.
4. 마지막으로 리포트가 생성이 되면 **PDF를 다운로드** 받습니다.

### 2. 분석 과정

```
📁 ZIP 파일 업로드
    ↓
🔍 Flask-A: 정적 분석 (Semgrep)
    ↓
🤖 Flask-B: AI 분석 (Claude)
    ↓
📊 리포트 생성 (PDF)
    ↓
💾 결과 저장 및 다운로드
```

### 3. 결과 확인

- **실시간 진행 상황**: 웹 인터페이스에서 확인
- **분석 결과**: JSON 형태로 다운로드
- **최종 리포트**: PDF 형태로 다운로드

## 🔧 API 엔드포인트

### 정적 분석 (Flask-A)

```bash
# 코드 분석 요청
POST /analyze
Content-Type: multipart/form-data
Body: file (ZIP)

# 분석 결과 조회
GET /results/{job_id}
```

### LLM 분석 (Flask-B)

```bash
# AI 기반 분석 요청
POST /analyze
Content-Type: application/json
Body: { "job_id": "uuid", "files": [...] }

# 분석 결과 조회
GET /results/{job_id}
```

## ⚙️ 설정 및 커스터마이징

### Semgrep 규칙 추가

`flask-a/analysis/detector.py`에서 Semgrep 규칙을 수정할 수 있습니다:

```python
# 커스텀 규칙 추가
custom_rules = [
    "--config=rules/custom-rules.yaml"
]
```

### LLM 모델 변경

`flask-b/llm_utils.py`에서 다른 LLM 모델을 사용할 수 있습니다:

```python
# Anthropic Claude 외 다른 모델 사용
def analyze_with_llm(code_content, vulnerability_info):
    # OpenAI GPT, DeepSeek 등으로 변경 가능
    pass
```

## 🐛 문제 해결

### 일반적인 문제

#### 1. API 키 오류

**증상**: Claude API 호출 실패
**해결**: 환경 변수에 올바른 API 키 설정

```bash
export ANTHROPIC_API_KEY=sk-ant-api03-your-actual-key-here
```

#### 2. 포트 충돌

**증상**: 서비스 시작 실패
**해결**: 사용 중인 포트 확인 및 변경

```bash
# 포트 사용 확인
netstat -ano | findstr :5000

# app.py에서 포트 변경
app.run(host='0.0.0.0', port=5001)  # 5000 → 5001로 변경
```

#### 3. 의존성 설치 오류

**증상**: pip install 실패
**해결**: Python 버전 확인 및 가상환경 사용

```bash
# Python 버전 확인
python --version

# 가상환경 생성 및 활성화
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 로그 확인

```bash
# Flask 서비스 로그
# 터미널에서 직접 확인

# 프론트엔드 로그
# 브라우저 개발자 도구 Console 탭에서 확인
```

## 🔒 보안 고려사항

### API 키 보안

- 환경 변수는 절대 Git에 커밋하지 마세요
- 프로덕션 환경에서는 환경 변수나 시크릿 관리 시스템 사용
- API 키는 정기적으로 로테이션

### 파일 업로드 보안

- ZIP 파일 크기 제한 설정
- 파일 타입 검증
- 악성 코드 실행 방지

### 네트워크 보안

- 프로덕션 환경에서는 HTTPS 사용
- 방화벽 설정으로 불필요한 포트 차단
- VPN 또는 프라이빗 네트워크 사용 권장

## 🚀 배포

### 프로덕션 환경

```bash
# 프로덕션 빌드
cd frontend
npm run build

# Flask 서비스 실행
cd flask-a
gunicorn -w 4 -b 0.0.0.0:5000 app:app

cd flask-b
gunicorn -w 4 -b 0.0.0.0:5001 app:app
```

### 개발 환경 설정

```bash
# Python 개발 의존성 설치
pip install black isort flake8 mypy pytest

# 코드 포맷팅
black .
isort .

# 린팅
flake8 .
mypy .

# 테스트 실행
pytest tests/
```
---
## 🙏 감사의 말

- **OWASP** - 보안 가이드라인 및 도구
- **Semgrep** - 정적 코드 분석 엔진
- **Anthropic** - Claude AI 모델
- **Flask** - Python 웹 프레임워크
- **React** - 사용자 인터페이스 라이브러리

## 팀

- **팀장**: 노경민
- **프론트엔드**: 권나희, 최민지
- **백엔드**: 권오현, 이승은, 정현범
- **AI/Security**: 강석경, 권나희, 노경민
---


<div align="center">

**LV.0 - AI로 보안을 더 스마트하게** 🚀

Made with ❤️ by [Guardians of the Open Source](https://github.com/Gaurdians-of-the-Open-Source)

</div>

