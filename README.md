# 내 일정

할 일 · 달력 · 근무 · 프로젝트 · 일기 · 식물 · 통계를 기록하는 웹앱. 빌드 없이 GitHub Pages로 배포하고, 데이터는 Supabase에 저장해 기기끼리 동기화합니다.

## 설치 순서
1. https://supabase.com 에서 새 프로젝트 생성
2. SQL Editor 에 `supabase/setup.sql` 전체를 붙여 넣고 Run
3. Authentication > Users > Add user 로 내 이메일·비밀번호 계정 만들기 (Auto Confirm 체크)
4. Project Settings > API 에서 Project URL 과 publishable(anon) key 를 복사해 `app.js` 맨 위 `SB_URL`, `SB_KEY` 에 넣기
5. 이 폴더를 내 GitHub 저장소에 올리고 Settings > Pages 에서 `main` 브랜치 / root 배포
6. 휴대폰에서 주소를 열고 "홈 화면에 추가"

## 내 것으로 바꾸기
- 근무지·시급·요일별 시간: `app.js` 의 `WORKPLACES`
- 프로젝트 약칭: `PROJ_SHORT`, 식물 초기 목록: `PLANT_SEED`
- 앱 이름: `index.html`, `manifest.webmanifest`, `app.js` 의 "내 일정"
- 가짜 데이터 미리보기: 주소 끝에 `?demo`
- 수정해서 올린 뒤 캐시가 안 바뀌면 `index.html` 의 `?v=` 숫자를 올리세요.
