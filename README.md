# 홍정의 포트폴리오 (Justice Hong — Portfolio)

음성인식(STT)·LLM 기반 의료 서비스를 클라이언트부터 서버·인프라까지 개발하고 운영하는
풀스택 개발자 홍정의의 포트폴리오 사이트입니다.

**Live:** https://justicehong.github.io/web-porfolio/

## 구성

| 섹션 | 내용 |
|---|---|
| About | 소개, 소속·직책, 연락처, 주요 지표 카드 |
| Work Experience | 2020년부터의 경력 (현재 ㈜퍼즐에이아이 서버파트 파트장) |
| Projects | 재직 기간 프로젝트 타임라인(간트) + 프로젝트 13건을 역시간순으로 정리 |
| Skills | Backend · Frontend/App · Infra/DB · AI/Voice · Ops 영역별 기술 태그 |
| Education | 교육·병역·전공 |
| Contact | 이메일 · GitHub |

병원·고객사 등 외부 기관명은 공개 사이트 특성상 익명으로 표기합니다.

## 기술 구성

- 정적 사이트: HTML / CSS / JavaScript (빌드 과정 없음)
- 베이스 템플릿: [Colorlib](https://colorlib.com) Portfolio 템플릿 (Bootstrap 4, jQuery) —
  [congchu/web-porfolio](https://github.com/congchu/web-porfolio) 구조에서 시작
- 커스텀 스타일은 `css/custom.css`에만 추가 (템플릿의 `css/style.css`는 수정하지 않음)
- 배포: GitHub Pages — `main` 브랜치 루트를 그대로 서빙 (Settings › Pages › Deploy from a branch).
  `main`에 push하면 1~2분 내 자동 반영됩니다. `.nojekyll`로 Jekyll 빌드를 생략합니다.

## 수정 방법

- 내용 수정: `index.html`의 각 섹션(`#about-section`, `#page-1`~`#page-4`, `#contact-section`)을 직접 편집
- 스타일 수정: `css/custom.css`
- 프로젝트 타임라인(`.timeline`): 축은 2025.04 ~ 현재(20개월) 기준이며 막대 위치는 `%`로 지정합니다.
  `left = (시작월 − 2025.04) ÷ 20`, 진행 중이면 `width = 100% − left`.
  프로젝트를 추가하면 `.tl-row` 한 줄과 상세 항목(`id="prj-*"`)을 함께 추가하고,
  2026.12 이후에는 축 길이(눈금 간격 15% = 3개월)도 함께 조정해야 합니다.
- 로컬 확인: `index.html`을 브라우저로 열거나 `python3 -m http.server 8000` 후 http://localhost:8000 접속

## 라이선스 / 크레딧

- 템플릿: © [Colorlib](https://colorlib.com), [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/) — 푸터의 제작자 표기는 유지합니다.
- 콘텐츠(텍스트·이미지): © 홍정의. 무단 전재를 금합니다.

_Last updated: 2026.11_
