# VCC Office Edition 1.1 Open Creator Beta

교육지원청·학교 업무프로그램을 **설계·진단·리팩터링·Python 하이브리드 전환**하는 바이브 코딩 코디네이터입니다.

## 바로 사용

GitHub Pages에서 `index.html`을 바로 실행할 수 있습니다.

- 새 업무도구 기획
- 4분류(유지·축소·폐지·자동화)
- 개발/검증/배포 요청서 생성
- 기존 HTML/ZIP 프로그램 진단
- Hybrid Architect
- Code Migration Mapper
- Migration Lab
- Skeleton / Migration Map / Migration Lab ZIP 생성

## 배포 채널

- **Web**: GitHub Pages
- **Windows Portable**: GitHub Releases
- **Source**: 이 저장소

Windows Release 패키지는 Python 3.14.8 Windows 64-bit embeddable runtime을 포함하도록 GitHub Actions가 자동 생성합니다. 사용 PC에 Python을 별도 설치할 필요가 없습니다.

## Windows 사용

Release에서 `VCC_Office_Edition_<version>_Windows_Portable.zip`을 내려받아 압축을 푼 뒤 `01_START_VCC.bat`을 실행합니다.

Bootstrap 소스 패키지를 직접 사용할 경우 처음 한 번 `00_SETUP_RUNTIME.bat`을 실행합니다.

## 개발·배포 원칙

- 브라우저 UI + 로컬 Python 처리 엔진
- `127.0.0.1` loopback only
- 고정 포트를 사용하지 않고 빈 포트 자동 선택
- 사용자 원본 파일 덮어쓰기 금지
- 기능 이관 시 회귀테스트 우선
- 태그 `v*` 생성 시 Windows Portable Release 자동 생성

## 버전

현재 정식 기준: **1.0.0**  
개발 기준 빌드: **v3.5 RC4 Windows 실기기 확인본**

## 라이선스 / 저작권

`LICENSE.txt`, `THIRD_PARTY_NOTICES.txt`를 확인하세요.

© 2026 강창원. All rights reserved.


## Open Creator Beta
- 자유 창작을 기본 시작점으로 제공합니다.
- 게임·학습앱·AI 비서·시뮬레이터·생활앱·센서/하드웨어 앱 등 자유 아이디어를 설계할 수 있습니다.
- 기존 업무도구 및 Migration Lab 기능은 그대로 유지합니다.