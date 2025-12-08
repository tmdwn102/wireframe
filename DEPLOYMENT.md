# 🚀 GitHub Pages 배포 가이드

ONFF Festival 웹사이트를 GitHub Pages에 배포하는 방법입니다.

## 📋 배포 전 체크리스트

- ✅ 모든 페이지 연결 확인 (5개 페이지)
- ✅ 이미지 폴더 준비 (`images/` 폴더 생성)
- ✅ 필수 이미지 5개 준비
- ⬜ GitHub 계정 준비

## 🎯 단계별 배포 방법

### 1단계: GitHub Repository 생성

1. GitHub.com 접속 및 로그인
2. 오른쪽 상단 `+` 버튼 클릭 → `New repository`
3. Repository 설정:
   ```
   Repository name: onff-festival-2025
   Description: ONFF Festival 2025 Official Website
   Public 선택 (GitHub Pages는 Public만 무료)
   ✅ Add a README file (체크 해제)
   ```
4. `Create repository` 클릭

### 2단계: 로컬에서 Git 설정

터미널 또는 Git Bash에서:

```bash
# 프로젝트 폴더로 이동
cd onff-festival

# Git 초기화
git init

# GitHub repository 연결 (본인의 username으로 변경!)
git remote add origin https://github.com/YOUR-USERNAME/onff-festival-2025.git

# 파일 추가
git add .

# 첫 커밋
git commit -m "Initial commit: ONFF Festival 2025 website"

# GitHub에 업로드
git branch -M main
git push -u origin main
```

### 3단계: GitHub Pages 활성화

1. GitHub repository 페이지에서 `Settings` 클릭
2. 왼쪽 메뉴에서 `Pages` 클릭
3. Source 설정:
   - Branch: `main` 선택
   - Folder: `/ (root)` 선택
4. `Save` 클릭
5. 2-3분 기다리면 배포 완료!

### 4단계: 웹사이트 접속

배포 완료 후 다음 주소로 접속:
```
https://YOUR-USERNAME.github.io/onff-festival-2025/
```

## 🖼️ 이미지 업로드 방법

### 방법 1: Git으로 업로드 (권장)

```bash
# images 폴더 생성
mkdir images

# 이미지 파일들을 images 폴더에 복사
# (poster.png, artist1.png, djset1.png, djset2.png, djset3.png)
# (gallery1.jpg ~ gallery8.jpg - 선택)

# Git에 추가 및 커밋
git add images/
git commit -m "Add festival images"
git push
```

### 방법 2: GitHub 웹에서 업로드

1. GitHub repository 페이지에서 `Add file` → `Upload files`
2. `images` 폴더 드래그 앤 드롭
3. `Commit changes` 클릭

## 🔄 웹사이트 업데이트하기

파일 수정 후:

```bash
git add .
git commit -m "Update: 수정 내용 설명"
git push
```

2-3분 후 자동으로 웹사이트에 반영됩니다.

## 🎨 커스텀 도메인 설정 (선택)

자신의 도메인이 있다면:

1. GitHub Pages 설정에서 `Custom domain` 입력
2. 도메인 제공업체에서 DNS 설정:
   ```
   Type: CNAME
   Name: www
   Value: YOUR-USERNAME.github.io
   ```

## ✨ 유용한 Git 명령어

```bash
# 현재 상태 확인
git status

# 변경 사항 확인
git diff

# 커밋 히스토리
git log --oneline

# 최근 커밋 취소 (조심!)
git reset --soft HEAD~1

# 원격 저장소 확인
git remote -v
```

## 🐛 문제 해결

### 페이지가 안 보여요
- Settings → Pages에서 `Save` 버튼을 다시 클릭
- 2-3분 기다려보기
- 브라우저 캐시 삭제 (Ctrl+Shift+R)

### 이미지가 안 보여요
- 이미지 파일명이 HTML과 정확히 일치하는지 확인
- 대소문자 구분 확인 (GitHub Pages는 대소문자 구분)
- `images/` 폴더가 올바른 위치에 있는지 확인

### Git push가 안 돼요
```bash
# Personal Access Token 필요 (2021년 이후)
# GitHub Settings → Developer settings → Personal access tokens
# repo 권한으로 토큰 생성 후 비밀번호 대신 사용
```

### 404 에러가 나요
- Repository 이름 확인
- 파일명이 `index.html`인지 확인 (소문자)
- Branch가 `main`으로 설정되어 있는지 확인

## 📱 모바일 테스트

배포 후 다양한 기기에서 테스트:
- 📱 iPhone Safari
- 🤖 Android Chrome
- 💻 Desktop (Chrome, Firefox, Safari)
- 📏 반응형 확인 (DevTools F12)

## 🔗 링크 공유

웹사이트 주소를 다음에 공유:
- Instagram Bio
- 페이스북 이벤트
- 포스터 QR코드
- 이메일 서명

---

**배포 완료 후:**
- Instagram: @onff_festival에서 웹사이트 링크 공유
- 친구들에게 테스트 요청
- 분석 도구 연결 (Google Analytics)

**문제가 있나요?**
- GitHub Community: https://github.community
- Stack Overflow: #github-pages 태그

즐거운 배포 되세요! 🎉
