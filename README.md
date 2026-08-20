# Cozy Shelter · 오늘의 카드

매일 한 장씩 뽑아보는 타로 카드 웹앱입니다. 정적 HTML/CSS/JS로만 되어 있으며 별도 빌드 과정이 없습니다.

**Live:** https://cozy-shelter-tarot.workers.dev <!-- 실제 배포 주소로 교체 -->

## 덱 (Decks)

- **고서 (Antique)** — `assets/v1`
- **밤 (Night)** — `assets/v2`
- **새벽 (Dawn)** — `assets/v3`

## 구조

```
index.html      메인 페이지 (전체 로직 포함)
assets/v1..v3   덱별 카드 이미지 (webp)
wrangler.jsonc  Cloudflare Worker 정적 배포 설정
```

## 배포

Cloudflare Workers(Git 연동)로 자동 배포됩니다. `main` 브랜치에 push하면 반영됩니다.

## 참고

이 저장소는 배포 전용 경량 저장소입니다. 원본 이미지 소스/작업 백업은 별도의 비공개 워크스페이스 저장소에서 관리합니다.
