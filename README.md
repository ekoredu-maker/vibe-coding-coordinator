# VCC · 바이브 코딩 코디네이터

교육지원청·학교 업무를 분석해 **기획 → 개발 요청서 → 기존 프로그램 진단 → Python Hybrid 전환 → Migration Map/Lab → 배포 점검**까지 이어 주는 업무도구 제작 코디네이터입니다.

## 배포 채널

- **Web / GitHub Pages**: 설치 없이 브라우저에서 바로 사용
- **Windows Portable / GitHub Releases**: Python Hybrid 기능과 로컬 파일 처리를 포함하는 실무용 배포판
- **Source / Repository**: 개발·검증·유지보수용 소스

현재 정식 배포 준비 후보는 **VCC Office Edition v3.5 RC**이며, 검증 완료 후 사용자에게는 **VCC Office Edition 1.0**으로 공개할 예정입니다.

## 주요 기능

- 반복 업무를 4서랍(유지·축소·폐지·자동화)으로 재구조화
- 업무 설명을 입력하면 개발 요청서와 검증 기준 자동 생성
- 기존 HTML/ZIP 프로그램 구조 진단
- Python Hybrid 전환 필요도·리팩터링·UI/UX 개선 필요도 분석
- 함수·이벤트 단위 Migration Mapper
- 저위험 JavaScript → Python 이관 후보 생성
- Hybrid 프로젝트 골격 및 검증 ZIP 생성
- 개인정보·민감정보 입력 위험 점검
- Windows Portable Release Gate 및 실행 진단

## 권장 사용법

### 1. 바로 사용하기
GitHub Pages에서 웹 버전을 실행합니다.

### 2. Windows 업무용
GitHub Releases에서 최신 `VCC_Windows_Portable_*.zip`을 내려받아 압축을 푼 뒤 실행합니다.

### 3. 개발·검증
이 저장소의 `main`은 배포 가능한 상태를 유지하고, 기능 변경은 별도 브랜치와 Pull Request에서 검증한 뒤 병합합니다.

## 배포 원칙

1. `main`에 병합하기 전에 자동 품질점검을 통과합니다.
2. `main` 병합 시 GitHub Pages를 자동 배포합니다.
3. 정식 버전은 `v1.0.0` 같은 태그로 관리합니다.
4. Windows Portable ZIP은 GitHub Releases에서 배포합니다.
5. 실제 학생·교직원·민원인 개인정보나 학교폭력·상담·건강·징계·인사 등 민감자료는 외부 AI에 그대로 입력하지 않습니다.

자세한 배포 절차는 [`docs/DEPLOYMENT.md`](docs/DEPLOYMENT.md)를 참고하세요.

## 저작권

© 2026 강창원. All rights reserved.
