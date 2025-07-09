<h1 align="center">🔐 LV.0: LLM Vulnerability Zero - Security Vulnerability Reporter</h1>
<p align="center"><strong>AI 기반 오픈소스 보안 취약점 리포팅 도우미</strong></p>

---

## 프로젝트 개요
**LV.0**는 오픈소스 프로젝트(GitHub 또는 압축 파일 형태)를 입력받아,  
정적 분석 도구와 LLM(Large Language Model)을 결합해 **보안 취약점을 자동 탐지 및 리포팅**하는  
웹 기반 보안 도우미 프로그램입니다.

취약 코드의 위험도를 평가하고, 개발자에게 **개선 방향까지 제시하는 실질적 보안 지원 도구**를 목표로 합니다.

---


## 핵심 기능

1. **코드 업로드 / GitHub 연동**
   - 사용자가 프로젝트를 업로드하거나 GitHub에서 직접 연동

2. **정적 분석 기반 취약점 필터링**
   - 오픈소스 정적 분석 도구를 활용한 1차 필터링

3. **LLM 기반 취약 코드 해석**
   - LLM을 통해 코드 맥락을 이해하고 위험도 평가 및 원인 설명

4. **자연어 기반 리포트 생성**
   - 취약점 요약, 위험도, 수정 방향 등을 포함한 리포트 자동 생성

5. **웹 GUI 제공**
   - 취약점 목록 및 상세 보기, 리포트 다운로드, 편리한 UX

---


## 사용 기술

- **LLM**: OpenAI GPT / Code LLM 기반 분석
- **정적 분석**: semgrep, bandit 등 오픈소스 도구
- **프론트엔드**: React, TailwindCSS
- **백엔드**: FastAPI, Python
- **DB/캐시**: MongoDB, Redis
- **배포**: Docker, MicroK8s, GitHub Actions

---

## 프로젝트 목적

> “보안은 어렵지 않다”  
LV.0는 복잡한 보안 분석 과정을 누구나 사용할 수 있도록 단순화하여,  
**개발자가 코딩에만 집중할 수 있는 환경**을 만드는 것을 목표로 합니다.

---

## 팀 정보

**팀명**: 가디언즈 오브 오픈소스  
**소속**: Dankook University Department of Cybersecurity 

**팀장**: 노경민

**인공지능 및 보안 개발**: 노경민, 강석경

**디자인 및 프론트엔드 개발**: 권나희, 최민지

**백엔드 개발**: 권오현, 이승은, 정현범

---

<p align="center">
  ⭐ <em>“AI로 보안을 더 쉽고, 더 똑똑하게.”</em> ⭐
</p>
