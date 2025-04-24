# MegazoneCloud Product Build Unit Organization
MegazoneCloud Product Build Unit

## 저장소 이름 생성 규칙
기본 규칙
- `{프로젝트 이름}-{서비스 이름}-{서비스 모듈 이름}`
- `프로젝트 이름`은 약어+소문자 작성
- `프로젝트 이름`이 없는 경우 다음 `프로젝트 이름` 생략 가능
- 각,이름에는 공백 대신 하이픈(-) 사용
- 저장소 이름에 대한 설명은 `README.md`에 기록
- 예시:
  - NBSS, Admin Center의 Backend 중, 인증 서비스 모듈
  - `nbss-admin-center-auth-controller-oauth2`

## 버저닝 규칙
기본 규칙
- `{Major version}.{Minor version}.{Patch version|Build version}`
- Major version
  - `0`부터 증가하는 숫자 사용
  - 기본적으로 상용 배포 버전은 `1`부터 시작
- Minor version
  - `0`부터 증가하는 숫자 사용
  - 구조 변경, 주요 기능 변경 등이 발생할 경우 증가 처리
- Patch version
  - `0`부터 증가하는 숫자 사용
  - 기능 수정에 따라 증가 처리
  - 관리를 위하여 기본적으로 순차 증가 처리
- Build version
  - 스냅샷 또는 nightly build 등에 대한 버전닝하는 경우 사용
  - `Commit hash` 또는 `YYYYmmDDhhMMss` 포맷의 타임스탬프 사용 가능
