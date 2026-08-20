# Cozy Shelter · 오늘의 카드

[![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-lightgrey.svg)](LICENSE)

매일 한 장씩 뽑아보는 타로 카드 웹앱입니다. 메이저 아르카나 22장을 **고서 · 밤 · 새벽** 3가지 테마 덱으로 지원합니다. 한국어 · English 2개 언어를 지원합니다. 정적 HTML/CSS/JS로만 되어 있으며 별도 빌드 과정이 없습니다.

**Live:** https://cozy-shelter-tarot.workers.dev <!-- 실제 배포 주소로 교체 -->

## 스크린샷

| 설정 | 카드 펼침 | 세 장 선택 완료 |
|---|---|---|
| ![설정](assets/screenshot/cozy-shelter-tarot-0.jpg) | ![카드 펼침](assets/screenshot/cozy-shelter-tarot-1.jpg) | ![세 장 선택 완료](assets/screenshot/cozy-shelter-tarot-2.jpg) |

| 카드 리딩 | 오늘의 요약 |
|---|---|
| ![카드 리딩](assets/screenshot/cozy-shelter-tarot-3.jpg) | ![오늘의 요약](assets/screenshot/cozy-shelter-tarot-4.jpg) |

## 덱 (Decks)

메이저 아르카나 22장 × 3가지 테마

- **고서 (Antique)** — 수묵풍 — `assets/v1`
- **밤 (Night)** — 유화풍 — `assets/v2`
- **새벽 (Dawn)** — 수채화풍 — `assets/v3`

## 구조

```
index.html          메인 페이지 (전체 로직 포함)
assets/v1..v3       덱별 카드 이미지 (webp)
assets/ci           Cozy Shelter 브랜드 심볼 (헤더/파비콘)
assets/screenshot   README용 스크린샷
wrangler.jsonc      Cloudflare Worker 정적 배포 설정
```

## 배포

Cloudflare Workers(Git 연동)로 자동 배포됩니다. `main` 브랜치에 push하면 반영됩니다.

## License

Copyright © 2026 Hanrim · Cozy Shelter. All Rights Reserved.

코드와 카드 아트워크를 포함한 이 저장소의 모든 콘텐츠는 원저작물이며, 저작권자의 사전 서면 허가 없이 복제·재배포·재사용(포크 후 재공개 포함)할 수 없습니다. 자세한 내용은 [LICENSE](LICENSE) 참고.

## 참고

이 저장소는 배포 전용 경량 저장소입니다. 원본 이미지 소스/작업 백업은 별도의 비공개 워크스페이스 저장소에서 관리합니다.
