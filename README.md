# 🎉 ONFF Festival 2025 웹사이트

ON과 OFF 사이, 새로운 커뮤니케이션을 탐구하는 문화 축제

## 📁 폴더 구조

```
onff-festival/
├── index.html          (홈페이지)
├── about.html          (페스티벌 소개)
├── lineup.html         (프로그램/라인업)
├── gallery.html        (갤러리)
├── timetable.html      (타임테이블)
├── tickets.html        (티켓 구매)
├── styles.css          (스타일시트)
├── README.md
└── images/
    └── main-hero.png   (메인 히어로 이미지) ⭐ 유일한 필수 이미지!
```

## 🎯 페이지 구성

### 🏠 HOME (index.html)
- **큰 히어로 이미지**: 전체 화면 메인 비주얼
- **FIVE ZONES**: 이모지로 표시된 5개 존 (🍔 🎉 💊 🎤)
- **LINEUP**: 아티스트 카드 (이모지 아이콘)

### 📖 ABOUT (about.html)
- 페스티벌 컨셉 소개
- ON/OFF SPACE 설명
- 일정 및 장소

### 🎵 PROGRAM (lineup.html)
- 아티스트 라인업
- 공연 시간 및 상세 정보
- 워크숍 프로그램

### 📸 GALLERY (gallery.html)
- 컨셉 비주얼 (색상 블록)
- 페스티벌 분위기 텍스트

### 🕐 TIMETABLE (timetable.html)
- 시간대별 상세 일정
- DAY 1, DAY 2 스케줄
- Zone 정보

### 🎫 TICKETS (tickets.html)
- 4가지 티켓 옵션
- 가격 및 구매 안내

## 🖼️ 필요한 이미지 - 단 1개!

### ⭐ 필수: main-hero.png

**저장 위치:** `images/main-hero.png`

**스펙:**
- 크기: 1920x800px (가로형 권장)
- 형식: PNG 또는 JPG
- 내용: "2025 ONFF FESTIVAL" 텍스트 + 캐릭터 일러스트레이션

**디자인 가이드:**
- 배경: 핑크색 (#FF4B9E)
- 일러스트: 라임 그린 (#D4FF00)
- 텍스트: "2025 ONFF FESTIVAL" 
- 스타일: 재미있고 에너제틱한 캐릭터
- 요소: 눈(eye) 모티브, 음악 관련 그래픽

**참고:** 나머지는 모두 이모지와 텍스트로 구성되어 있어서 이미지가 필요 없습니다!

## 🎨 색상 팔레트

```css
라임 그린: #D4FF00
핫 핑크: #FF4B9E  
네비게이션: #333333
배경: #ebebeb
텍스트: #2c2c2c
```

## 🚀 빠른 시작

### 1. 폴더 설정

```bash
# images 폴더 생성
mkdir images

# main-hero.png 파일을 images 폴더에 넣기
```

### 2. 로컬에서 실행

**Visual Studio Code 사용:**
1. Live Server 확장 프로그램 설치
2. `index.html` 우클릭 → "Open with Live Server"
3. 브라우저가 자동으로 열림

**일반 브라우저:**
- `index.html` 파일을 더블클릭

### 3. GitHub Pages 배포

```bash
# Git 초기화
git init
git add .
git commit -m "Initial commit: ONFF Festival 2025"

# GitHub 업로드 (본인 username으로!)
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/onff-festival-2025.git
git push -u origin main

# GitHub Pages 활성화
# Settings → Pages → Source: main → Save
```

**배포 후 접속 주소:**
```
https://YOUR-USERNAME.github.io/onff-festival-2025/
```

## ✨ 주요 특징

### 📱 모든 기기에서 동일한 레이아웃
- **데스크톱, 태블릿, 모바일 모두 같은 화면**
- 모바일에서는 확대/축소로 볼 수 있음 (핀치 줌)
- 가로 스크롤 지원
- 일관된 디자인 경험

### 🎨 이모지 아이콘 사용
- 이미지 없이도 화려한 디자인
- 빠른 로딩 속도
- 유지보수 간편

### 🔗 완벽한 네비게이션
```
HOME → ABOUT → PROGRAM → GALLERY → TIMETABLE → TICKETS
```

### 🎯 핵심 기능
- ✅ 6개 페이지 완성
- ✅ 반응형 디자인
- ✅ 라임 그린 & 핑크 테마
- ✅ 이모지 기반 아이콘
- ✅ Footer 포함
- ✅ 호버 애니메이션

## 🎭 이모지 사용 위치

### 홈페이지
- 🍔 Food Zone
- 🎉 Festive Zone  
- 💊 Capsule Zone
- 🎤 Voice Zone
- 🎵 Luna Park
- 🎧 DJ NEON
- 🎸 R&B Collective
- 🎭 EYE DJ

### 갤러리
- 색상 블록 + 텍스트로 구성
- 이미지 없이 컨셉 전달

### 프로그램
- 🎵 🎧 🎸 🎭 아이콘으로 아티스트 표현

## ⚙️ 커스터마이징

### 색상 변경
`styles.css` 파일 상단:
```css
:root {
    --lime-green: #D4FF00;  /* 원하는 색으로 */
    --hot-pink: #FF4B9E;    /* 원하는 색으로 */
}
```

### 텍스트 수정
각 HTML 파일을 열어 원하는 내용으로 수정

### 이모지 변경
HTML 파일에서 이모지만 바꾸면 됨:
```html
<div class="zone-icon-emoji">🍕</div>  <!-- 원하는 이모지로 -->
```

## 📌 체크리스트

배포 전 확인:
- ✅ 모든 HTML 파일 (6개)
- ✅ styles.css
- ✅ images 폴더 생성
- ⭐ **main-hero.png 준비** (유일한 필수!)

## 💡 팁

### 📱 모바일에서 보기
- **핀치 줌**: 두 손가락으로 확대/축소
- **가로 스크롤**: 좌우로 슬라이드
- **세로 보기**: 화면을 회전시켜서 가로로 보는 것 추천
- 데스크톱과 동일한 레이아웃이 유지됩니다

### 메인 히어로 이미지 제작
1. **Canva 사용**: 1920x800px 크기로 제작
2. **Figma 사용**: 배경색 #FF4B9E 적용
3. **일러스트**: Freepik, Flaticon 무료 리소스 활용
4. **텍스트**: 굵은 폰트로 "2025 ONFF FESTIVAL"
5. **색상**: 라임 그린 (#D4FF00) 강조

### 이미지 없이도 완성도 있는 이유
- 이모지가 모든 아이콘 역할
- 색상 블록으로 섹션 구분
- 텍스트 중심 정보 전달
- 빠른 로딩 속도

## ❓ 자주 묻는 질문

**Q: 이미지 1개만 있으면 정말 완성되나요?**
A: 네! main-hero.png만 있으면 모든 페이지가 완벽하게 작동합니다.

**Q: 모바일에서 레이아웃이 작게 보여요**
A: 정상입니다! 핀치 줌(두 손가락으로 확대)으로 원하는 크기로 볼 수 있어요. 모든 기기에서 동일한 레이아웃을 유지합니다.

**Q: 모바일 반응형은 없나요?**
A: 의도적으로 모든 기기에서 동일한 레이아웃을 보여줍니다. 이렇게 하면 어떤 기기에서도 같은 디자인을 경험할 수 있어요.

**Q: 나중에 더 많은 이미지를 추가하고 싶어요**
A: 언제든지 가능합니다! 이미지를 images 폴더에 추가하고 HTML을 수정하세요.

**Q: 이모지가 안 보이면?**
A: 최신 브라우저를 사용하세요. 대부분의 브라우저에서 지원됩니다.

**Q: GitHub Pages가 작동하지 않아요**
A: Settings → Pages에서 Source가 main 브랜치로 설정되었는지 확인하세요.

## 📞 문의

- Email: info@onff-festival.com
- Instagram: @onff_festival

---

**제작:** ONFF Festival 2025  
**버전:** 이미지 최소화 버전 (메인 히어로만 필요!)

단 1개의 이미지로 완성되는 페스티벌 웹사이트! 🎉✨
