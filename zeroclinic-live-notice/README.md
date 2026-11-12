# 김남백 웨비나 단톡방 운영 페이지 (Vercel 배포용)

## 들어 있는 것
- index.html : 운영 페이지 (전략 · 할 일 · 공지 문구 복사 · GIF 다운로드)
- gif/ : 단톡방 GIF 15종 (m01 ~ m15)
- vercel.json : 검색 노출 차단 헤더, GIF 캐시 설정
- robots.txt : 검색 엔진 수집 차단

## 배포 방법 1 · 드래그 앤 드롭 (가장 쉬움)
1. vercel.com 로그인 → Add New → Project
2. 이 폴더(zeroclinic-live)를 그대로 끌어다 놓기
3. Framework Preset: Other, Build Command 비워 두기 → Deploy

## 배포 방법 2 · Vercel CLI
```
npm i -g vercel
cd zeroclinic-live
vercel --prod
```

## 주의
- 배포 주소를 아는 사람은 누구나 볼 수 있습니다. 내부 전략이 들어 있으니
  주소는 팀 안에서만 공유하고, 가능하면 Vercel의 Password Protection(유료 플랜)이나
  Vercel Authentication(팀 멤버만 접근)을 켜 주세요.
- 할 일 체크 상태는 각자 브라우저에만 저장됩니다.
- 복사 버튼은 https 주소에서만 동작합니다 (Vercel 기본 주소는 https).
