# 2026 플레이샵

아난티 앳 부산 1박 2일 일정 초안 + 투표 페이지.

## 로컬 확인

```bash
open index.html
```

정적 HTML 하나로 동작합니다. 별도 빌드 필요 없음.

## GitHub Pages 배포

`main` 브랜치에 push 하면 `.github/workflows/deploy.yml`이 GitHub Pages로 자동 배포합니다.

1. 저장소 만들기 (예: `kakao-grace-j/playshop-2026`)
2. `git init && git add . && git commit -m "init"`
3. `git remote add origin https://github.com/kakao-grace-j/playshop-2026.git`
4. `git push -u origin main`
5. GitHub 저장소 → Settings → Pages → Source를 **GitHub Actions**로 설정
6. Actions 탭에서 배포 완료 확인 → `https://kakao-grace-j.github.io/playshop-2026/` 접속

## 투표 데이터

현재는 브라우저 `localStorage`에만 저장됩니다.
플레이샵 현장에서 실시간 집계가 필요하면 서버(Runway + SQLite/PVC 또는 Google Sheets Web App) 연동으로 교체합니다.
