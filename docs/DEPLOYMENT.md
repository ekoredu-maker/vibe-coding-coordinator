# VCC 배포 가이드

## 배포 구조

VCC는 역할을 분리해 배포합니다.

- **GitHub Pages**: 웹 실행판
- **GitHub Releases**: Windows Portable ZIP 및 체크섬
- **GitHub Repository**: 소스와 자동화 설정

## GitHub Pages

`main` 브랜치에 배포용 변경이 병합되면 `.github/workflows/pages.yml`이 실행됩니다.

저장소의 **Settings → Pages → Build and deployment → Source**를 `GitHub Actions`로 한 번 설정하면 이후에는 워크플로가 자동 배포합니다.

## 배포 전 점검

Pull Request에서는 `.github/workflows/quality-gate.yml`이 다음 기본 항목을 확인합니다.

- `index.html` 존재 여부
- HTML 기본 문서 구조
- 중복 DOM id 여부
- JavaScript가 참조하는 DOM id 누락 여부

VCC Office Edition 1.0 전환 커밋에서는 Python 엔진·Local API·Migration ZIP까지 검증하는 Release Gate를 추가합니다.

## 정식 릴리스 절차

1. Release Candidate를 Windows PC에서 실제 실행합니다.
2. 전체 Release Gate를 통과시킵니다.
3. Pull Request를 `main`에 병합합니다.
4. GitHub Pages가 정상 배포되었는지 확인합니다.
5. `v1.0.0` 태그를 생성합니다.
6. Release workflow가 Windows Portable ZIP과 SHA-256 파일을 생성하는지 확인합니다.
7. 다른 Windows PC에서 Portable ZIP을 다시 실행해 최종 확인합니다.

## 버전 규칙

- `1.0.0`: 최초 정식판
- `1.0.1`: 오류 수정
- `1.1.0`: 하위 호환 기능 추가
- `2.0.0`: 구조 또는 호환성의 큰 변경

## 운영 원칙

`main`은 언제든 배포 가능한 상태를 유지하고, 개발 작업은 별도 브랜치에서 진행합니다.
