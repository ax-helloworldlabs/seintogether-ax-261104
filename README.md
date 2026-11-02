# AX 레시피 생성형 AI 활용

현장의 반복 업무를 진단하고 개인화 AI 비서를 기획·제작해 현업 적용안까지 만드는 8시간 실습 과정의 수강생 안내 페이지입니다. 2026년 11월 4일(수) 09:00–18:00, 세인투게더빌딩 5층 쇼룸.

## 배포 방법 (GitHub Pages)

1. `ax-helloworldlabs` 조직에 새 저장소를 만듭니다. 저장소 이름이 주소가 됩니다. 예: `ax-recipe-genai` → `https://ax-helloworldlabs.github.io/ax-recipe-genai/`
2. 이 폴더 안의 파일을 모두 저장소 최상위에 올립니다. `.nojekyll`(숨김 파일)도 함께 올려 주세요.
3. 저장소 **Settings → Pages**에서 Source를 `Deploy from a branch`, Branch를 `main` / `/(root)`로 저장합니다.
4. 1–2분 뒤 위 주소에서 페이지가 열리는지 확인합니다.

## 무엇을 어디서 고치나

| 고칠 내용 | 파일 · 위치 |
|---|---|
| 페이지 제목·검색/공유 설명 | `index.html` `<head>`의 `<title>`, `meta description`, `og:*` |
| 사업명·과정명·소개 문구 | `index.html` `section.hero` (`.eyebrow`, `.course-label`, `h1`, `.hero-sub`, `.hero-desc`) |
| 날짜·시간·장소 요약 띠 | `index.html` `.event-strip` |
| 신분증 안내 배너 | `index.html` `.id-notice` |
| 준비물 카드 | `index.html` `#preparation` `.prep-card` |
| 일정 카드·장소·지도 링크 | `index.html` `#place` (`.schedule-card`, `.venue-card`) |
| 주소 복사 버튼의 주소 | `script.js` 첫 줄 `const address` |
| 커리큘럼 모듈(시간·과목명·세부 내용) | `index.html` `#curriculum` 의 `<details class="module">` 5개 |
| 점심시간 줄 | `index.html` `.lunch-break` |
| 교육 결과물 3가지 | `index.html` `.outcome` |
| 사전 안내 PDF·SafariON·카카오 채널·전화 | `index.html` `#resources`, 파일은 `assets/course-guide.pdf` |
| 하단 사업명·운영기관·홈페이지 | `index.html` `<footer>` |
| 모바일 하단 고정 바 | `index.html` `.mobile-bar` |
| Claude 유료 계정 1개월 지원·계정 정보 안내 | `index.html` `#support` |
| 색상 | `styles.css` 첫 줄 `:root` (`--green`, `--lime`, `--ink` 등) |

CSS·JS를 고친 뒤에는 `index.html`의 `styles.css?v=20261104-6`, `script.js?v=20261104-1` 끝 숫자를 1 올려 주세요(브라우저 캐시 갱신).

## 아직 넣지 않은 정보 / 확인할 정보

- **교육장 출입 안내**: 세인투게더빌딩 출입 방법·가까운 역 정보가 없어 넣지 않았습니다. 필요하면 `#place` `.venue-card`의 주소 아래에 `<p class="elevator-note">※ …</p>` 형태로 추가하세요.
- **강사명**: 시간표(남윤진)에 있으나 지난 페이지와 같이 표기하지 않았습니다.
- **지난 과정(ax-kit-sales) 공통 정보를 재사용**: 아래 항목은 이번 시간표에는 없고 지난 과정 페이지의 값을 그대로 가져왔습니다. 이번 과정에서 달라지면 수정하세요.
  - 준비물(실물·모바일 신분증 필수·캡처본 불가, 개인 노트북, 노트북 충전기)
  - 실습 도구 태그 "Claude Cowork 실습", Claude 유료 계정 1개월 지원 안내
  - 교육 사전 안내 PDF(`assets/course-guide.pdf`, SafariON 공통 이용 가이드)
  - SafariON 교안·실습 자료 링크(아이디 = 교육 안내를 받은 메일 주소, 비밀번호 = `safarion`), 카카오톡 채널 Hello, AX, 전화 070-8833-7771
