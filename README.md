# inch260605# Copilot Studio 챗봇 - 커스텀 디자인

Microsoft Copilot Studio를 활용하여 만든 파스텔톤 커스텀 디자인 챗봇입니다. 부드러운 글씨체와 아름다운 색상 조합으로 사용자 경험을 극대화했습니다.

## 🎨 특징

✨ **커스텀 디자인**
- 파스텔톤 색상 (#DE8DE2, #80B9EF)
- 부드러운 그라데이션 배경
- 둥근 모서리와 소프트 그림자

🎯 **최적화된 레이아웃**
- 가로: 화면의 50%
- 높이: 화면의 2/3
- 중앙 정렬로 깔끔한 UI

📱 **반응형 디자인**
- 데스크톱: 50% 너비
- 태블릿: 70% 너비
- 모바일: 95% 너비 (자동 조정)

✍️ **우아한 타이포그래피**
- Google Fonts 적용
- Noto Sans KR (한글)
- Poppins (영문)

## 🚀 시작하기

### 설치 방법

1. 이 레포지토리를 클론합니다:
```bash
git clone https://github.com/your-username/copilot-studio-chatbot.git
cd copilot-studio-chatbot
```

2. `index.html` 파일을 웹 브라우저에서 엽니다:
   - 로컬: 파일을 직접 더블클릭
   - 또는 간단한 HTTP 서버로 실행:
```bash
python -m http.server 8000
```

3. `http://localhost:8000`에서 확인합니다.

### 웹에 배포

#### GitHub Pages 사용
1. `Settings` > `Pages`로 이동
2. `Source`에서 `main` 브랜치 선택
3. `https://your-username.github.io/copilot-studio-chatbot/`에서 접근

#### 다른 호스팅 서비스
- Netlify, Vercel, Firebase Hosting 등에 업로드 가능

## 📝 파일 구조

```
copilot-studio-chatbot/
├── README.md          # 이 파일
├── index.html         # 메인 HTML 파일
└── LICENSE           # 라이선스
```

## ⚙️ 커스터마이징

### 색상 변경

`index.html` 파일에서 다음 부분을 수정합니다:

```html
<!-- 배경 색상 변경 -->
background: linear-gradient(135deg, #f0e4f0 0%, #e8f4ff 100%);

<!-- 래퍼 배경 변경 -->
background: linear-gradient(135deg, rgba(222, 141, 226, 0.1) 0%, rgba(128, 185, 239, 0.1) 100%);
```

### 크기 조정

```css
.chatbot-wrapper {
    width: 50%;      /* 너비 조정 */
    height: 66.67%;  /* 높이 조정 */
}
```

### 글씨체 변경

Google Fonts에서 원하는 폰트를 선택하고 `<link>` 태그를 수정합니다:

```html
<link href="https://fonts.googleapis.com/css2?family=YOUR_FONT&display=swap" rel="stylesheet">
```

### 챗봇 URL 변경

Copilot Studio에서 제공받은 새로운 URL로 `src` 속성을 수정합니다:

```html
<iframe 
    src="YOUR_COPILOT_STUDIO_URL"
    ...
></iframe>
```

## 🔐 보안 주의사항

- 이 버전은 **공개 챗봇**용입니다
- 사용자 인증이 필요한 경우, **토큰 기반 인증**을 추가하세요
- 민감한 정보는 환경 변수로 관리하세요

### 토큰 기반 인증 추가 (선택사항)

```html
<script>
  async function getAuthToken() {
    const response = await fetch('YOUR_TOKEN_ENDPOINT_URL', {
      method: 'POST',
      headers: { 'Content-Type': 'application/json' },
    });
    const data = await response.json();
    return data.token;
  }
</script>
```

## 📋 요구사항

- 최신 웹 브라우저 (Chrome, Firefox, Safari, Edge)
- 인터넷 연결 (Copilot Studio 서버 접속용)
- JavaScript 활성화

## 💻 브라우저 지원

| 브라우저 | 지원 |
|---------|------|
| Chrome  | ✅   |
| Firefox | ✅   |
| Safari  | ✅   |
| Edge    | ✅   |
| IE 11   | ❌   |

## 🤝 기여 방법

1. Fork합니다
2. Feature 브랜치를 생성합니다 (`git checkout -b feature/amazing-feature`)
3. 변경사항을 커밋합니다 (`git commit -m 'Add amazing feature'`)
4. 브랜치에 Push합니다 (`git push origin feature/amazing-feature`)
5. Pull Request를 생성합니다

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 있습니다. `LICENSE` 파일을 참조하세요.

## 📧 문의

문제가 있거나 제안이 있으면 [Issues](https://github.com/your-username/copilot-studio-chatbot/issues)를 열어주세요.

## 🙏 감사의 말

- Microsoft Copilot Studio
- Google Fonts

---

**Made with ❤️ using Copilot Studio**천교육청 AI융합교육원 코파일럿스튜디오 테스트입니다
