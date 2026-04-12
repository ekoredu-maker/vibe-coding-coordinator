# 바이브 코딩 코디네이터

이 저장소는 **바이브 코딩 코디네이터**를 GitHub에 올리고, GitHub Pages로 바로 배포할 수 있도록 정리한 패키지입니다.

## 포함 파일

- `index.html` : 메인 실행 파일
- `README.md` : 저장소 소개 및 배포 방법
- `.nojekyll` : GitHub Pages 정적 배포 안정화용 파일
- `.gitignore` : 기본 무시 규칙
- `LICENSE.txt` : 권리표시 문구

## 앱 개요

이 도구는 다음 작업을 한 화면에서 수행하도록 설계되어 있습니다.

- 프로젝트 기본 정보 입력
- 문제, 목표, 기능 흐름, 예외상황 정리
- 자동 품질 점검
- AI 작업지시서 생성
- 복사 / TXT 저장 / JSON 내보내기 / JSON 가져오기

## 로컬 실행

1. 이 저장소를 다운로드합니다.
2. `index.html` 파일을 브라우저에서 엽니다.
3. 바로 사용할 수 있습니다.

## GitHub 업로드 방법

1. GitHub에서 새 저장소를 만듭니다.
2. 이 패키지 안의 파일 전체를 저장소 루트에 업로드합니다.
3. 기본 문서는 `index.html` 이므로 바로 정적 사이트로 사용할 수 있습니다.

## GitHub Pages 배포 방법

1. 저장소의 **Settings** 로 이동합니다.
2. 왼쪽 메뉴에서 **Pages** 를 엽니다.
3. **Build and deployment** 에서 Source를 **Deploy from a branch** 로 선택합니다.
4. Branch는 **main**, Folder는 **/ (root)** 를 선택합니다.
5. 저장 후 몇 분 뒤 배포 주소가 생성됩니다.

## 저작권

앱 배포본 기본 표시는 아래와 같이 반영했습니다.

`© 2026 강창원. All rights reserved.`

프로그램 내 `개발자/기획자 이름`을 바꾸면 생성되는 문구와 하단 표시는 함께 바뀌지만, 배포본 기본값은 강창원으로 설정되어 있습니다.

## 권장 저장소 설명 문구

브라우저에서 바로 실행되는 단일 HTML 기반 AI 작업지시서 생성 도구

## 권장 저장소 이름 예시

- `vibe-coding-coordinator`
- `vibe-coding-coordinator-web`
- `ai-prompt-coordinator`
