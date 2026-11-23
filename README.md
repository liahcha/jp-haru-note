# 🇯🇵 HARU 일본어 스마트 학습 노트

PC · 아이패드(iPad) · 스마트폰(iOS/Android) 어디서나 학습하는 개인 맞춤형 일본어 웹앱입니다.

## 📁 깔끔한 역할 분리 구조
- **`index.html`** (순수 웹앱, 내장 데이터 없음): `data/manifest.json`과 `data/yyyyMMdd.json`을 자동으로 읽어와 **노트 · 30문항 퀴즈 · 단어장 · 문법노트**를 렌더링합니다.
- **`data/` 폴더**: 날짜별 수업 노트 JSON(`20260828.json` ~ `20261117.json`) + 목록 파일(`manifest.json`). 새 수업이 생기면 **`index.html`은 건드리지 않고 `data/` 폴더에만 새 날짜 JSON과 `manifest.json`을 업로드**하면 모든 메뉴가 자동 업데이트됩니다.
- **`icons/` & `manifest.webmanifest`**: 아이패드·스마트폰 홈 화면 설치용 PWA 앱 아이콘.
- **구글 시트 (`Study note_HARU`)**: 오직 문제풀이 결과 및 오답 분석 전용 (`문제풀이_기록` + `학습_요약`).
