# 한글춤 (Hangul Dance) 🎨

한글 타이포그래피를 활용한 인터랙티브 디지털 아트 웹 애플리케이션입니다.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-web-green.svg)

## ✨ 주요 기능

### 🎬 텍스트 애니메이션
- 한글 텍스트를 파티클 형태로 애니메이션화
- 강도, 방향, 크기, 간격 조절 가능
- 부드러운 탄성 애니메이션 효과

### 🎨 커스터마이징
- **폰트**: 21종의 아름다운 한글 폰트 지원
- **색상**: 배경색과 글자색 자유롭게 선택
- **배경**: 단색/이미지/비디오 업로드 지원 (비율 자동 조정)
- **캔버스 크기**: 정사각형, PPT, 릴스, 가로 등 다양한 프리셋

### 🎞️ 슬라이드 관리
- 여러 슬라이드 생성 및 관리
- 슬라이드 간 자유로운 전환
- 실행 취소/다시 실행 기능
- 슬라이드 삭제 (최소 1개 유지)
- 전체 초기화 기능

### 📹 녹화 기능
- **GIF 형식**: gif.js 라이브러리 활용
- **WebM 형식**: MediaRecorder API 활용 (기본값)
- 자동 다운로드 기능

### 🌍 다국어 지원
- 한국어/영어 전환 기능
- localStorage를 통한 언어 설정 저장

### 🌙 테마 모드
- 다크 모드 (기본값)
- 라이트 모드
- localStorage를 통한 테마 설정 저장

## 🚀 시작하기

### 필요 사항
- 모던 웹 브라우저 (Chrome, Firefox, Safari, Edge)
- 인터넷 연결 (폰트 및 라이브러리 로드)

### 사용 방법

1. **텍스트 입력**
   - 상단 입력창에 한글 텍스트 입력
   - 실시간으로 캔버스에 애니메이션 표시

2. **스타일 조정**
   - 배경색/글자색 선택
   - 21가지 폰트 중 선택
   - 배경 이미지/비디오 업로드 (선택사항)

3. **애니메이션 조절**
   - **강도**: 애니메이션 움직임 크기
   - **방향**: 가로/세로 방향 비율
   - **크기**: 글자 크기 (10-150)
   - **간격**: 글자 사이 간격

4. **녹화 및 저장**
   - GIF 또는 WebM 형식 선택
   - "녹화 시작" 버튼 클릭
   - 다시 클릭하여 중지 및 자동 다운로드

5. **다국어 전환**
   - 우측 하단 "KOR/ENG" 버튼 클릭
   - 한국어 ↔ 영어 전환

6. **테마 변경**
   - 우측 하단 달/해 아이콘 클릭
   - 다크 모드 ↔ 라이트 모드 전환

## 🛠️ 기술 스택

- **Frontend**: Vanilla JavaScript
- **Styling**: Tailwind CSS (CDN)
- **Canvas**: HTML5 Canvas API
- **Recording**: 
  - gif.js (GIF)
  - MediaRecorder API (WebM)
- **Fonts**: Google Fonts (21종)

## 📁 프로젝트 구조

```
/
├── index.html          # 메인 애플리케이션 파일
├── gif.worker.js       # GIF 녹화 워커
├── replit.md          # 프로젝트 문서 (한글)
└── README.md          # 프로젝트 문서 (영문 포함)
```

## 🎯 지원 폰트

1. Noto Sans KR
2. Black Han Sans
3. Jua
4. Do Hyeon
5. Nanum Gothic
6. Nanum Pen Script
7. Gothic A1
8. Nanum Myeongjo
9. East Sea Dokdo
10. Gaegu
11. Gamja Flower
12. Gugi
13. Hi Melody
14. Single Day
15. Song Myung
16. Stylish
17. Sunflower
18. Yeon Sung
19. Grandiflora One
20. Diphylleia
21. Black And White Picture

## 📐 캔버스 크기 프리셋

- **정사각형**: 1920x1920px
- **PPT**: 1920x1080px (16:9)
- **릴스**: 1080x1920px (9:16)
- **가로**: 4000x3000px (4:3)

## 🔧 주요 기능 상세

### 실행 취소/다시 실행
- 각 슬라이드별 독립적인 히스토리 관리
- 상태 변경 시 자동 저장
- 직관적인 화살표 버튼

### 슬라이드 관리
- 슬라이드 추가: 새 슬라이드 생성 (기본값: '한글춤')
- 슬라이드 삭제: 현재 슬라이드 제거 (최소 1개 유지)
- 이전/다음: 슬라이드 탐색
- 초기화: 모든 슬라이드 삭제 후 기본 슬라이드 1개 복원

### 배경 이미지/비디오
- 이미지: 캔버스 비율에 맞게 자동 스케일링 (contain)
- 비디오: 자동 재생 및 반복
- 지원 형식: 
  - 이미지: JPG, PNG, GIF 등
  - 비디오: MP4, WebM 등

## 📱 반응형 디자인

- **모바일 최적화**
  - ≤640px: 290px 여유 공간 확보
  - ≤768px: 260px 여유 공간 확보
  - 터치 친화적 UI (버튼 크기 44px+)
  
- **데스크톱 최적화**
  - 넓은 화면에서 편안한 작업 공간
  - 키보드/마우스 최적화 인터랙션

## 🌐 브라우저 지원

- Chrome (권장)
- Firefox
- Safari
- Edge

## 📝 라이센스

이 프로젝트는 개인 및 교육 목적으로 자유롭게 사용할 수 있습니다.

## 👨‍💻 제작자

**created by. 교육뮤지컬 꿈꾸는 치수쌤**

[웹사이트 방문하기](http://litt.ly/chichiboo)

## 🙏 감사의 말

한글을 사랑하고 아끼는 마음으로 만들었습니다 ❤️

---

Made with ❤️ for Hangul Typography
