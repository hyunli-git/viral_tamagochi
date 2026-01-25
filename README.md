# 🥚 타마고치 - 온라인 디지털 펫 게임

귀여운 디지털 펫을 키워보세요! 아날로그 감성의 레트로 스타일 다마고치 게임입니다.

![타마고치 게임 미리보기](preview.png)

## ✨ 특징

- **레트로 아날로그 디자인**: 90년대 다마고치 느낌의 UI
- **CRT 스캔라인 효과**: 옛날 LCD 화면 느낌
- **4가지 스탯 관리**: 배고픔, 행복도, 에너지, 청결도
- **레벨업 시스템**: 펫을 잘 돌보면 경험치 획득 & 레벨업
- **자동 저장**: 로컬 스토리지에 게임 자동 저장
- **오프라인 시간 반영**: 접속하지 않은 동안의 시간도 반영
- **반응형 디자인**: 모바일/데스크톱 모두 지원

## 🎮 게임 방법

1. **먹이주기 🍖**: 배고픔 스탯을 채워줍니다
2. **놀아주기 ⚽**: 행복도를 올리지만 에너지가 소모됩니다
3. **재우기 😴**: 에너지를 회복합니다
4. **청소하기 🧹**: 청결도를 올리고 💩를 치웁니다

## ⚠️ 주의사항

- 배고픔이나 행복도가 0이 되면 펫이 죽습니다!
- 정기적으로 돌봐주세요

## 🚀 시작하기

### 로컬에서 실행
```bash
# 간단한 HTTP 서버로 실행
npx serve .

# 또는 Python으로
python -m http.server 8000
```

브라우저에서 `http://localhost:8000` 접속

### 배포하기

정적 파일이므로 어디서든 호스팅 가능합니다:
- **GitHub Pages** (무료)
- **Netlify** (무료)
- **Vercel** (무료)
- **Firebase Hosting**
- **AWS S3 + CloudFront**

## 💰 Google AdSense 설정

1. [Google AdSense](https://www.google.com/adsense) 가입
2. 사이트 승인 받기 (콘텐츠가 충분해야 함)
3. `index.html`에서 AdSense 코드 수정:

```html
<!-- head 태그 내 주석 해제 후 YOUR_PUBLISHER_ID 교체 -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_PUBLISHER_ID" crossorigin="anonymous"></script>
```

4. 광고 단위 생성 후 광고 영역에 코드 삽입:

```html
<!-- 상단 배너 (728x90) -->
<ins class="adsbygoogle"
     style="display:inline-block;width:728px;height:90px"
     data-ad-client="ca-pub-YOUR_PUBLISHER_ID"
     data-ad-slot="YOUR_AD_SLOT"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
```

### AdSense 승인 팁

- 개인정보처리방침 페이지 추가
- 이용약관 페이지 추가
- 충분한 오리지널 콘텐츠
- 명확한 네비게이션
- 모바일 친화적 디자인 ✅

## 📁 프로젝트 구조

```
tamagochi/
├── index.html      # 메인 게임 파일 (HTML + CSS + JS)
├── README.md       # 프로젝트 설명
└── privacy.html    # 개인정보처리방침 (AdSense용, 선택사항)
```

## 🔧 커스터마이징

### 색상 변경
`index.html`의 CSS 변수 수정:
```css
:root {
    --bg-color: #e8dcc4;      /* 배경색 */
    --device-color: #7eb8a2;  /* 기기 색상 */
    --screen-bg: #9bbc0f;     /* 화면 배경 (게임보이 느낌) */
    --text-dark: #0f380f;     /* 텍스트 색상 */
}
```

### 게임 밸런스 조정
JavaScript의 `gameTick()` 함수에서 스탯 감소량 조절:
```javascript
gameState.hunger = Math.max(0, gameState.hunger - 2);     // 배고픔 감소 속도
gameState.happiness = Math.max(0, gameState.happiness - 1.5); // 행복도 감소 속도
```

## 📄 라이선스

MIT License - 자유롭게 사용, 수정, 배포 가능

## 🤝 기여

버그 리포트나 기능 제안은 이슈로 남겨주세요!

---

Made with ❤️ for 다마고치 lovers
