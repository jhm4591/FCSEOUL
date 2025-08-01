
# ⚽ FC SEOUL 웹사이트 리뉴얼 포트폴리오

> FC서울 공식 웹사이트를 리뉴얼한 프로젝트로, 전체 UI/UX 구조를 현대적이고 사용자 친화적으로 개선하였습니다.

---
## 🐫 팀 정보

### 👥 구성 인원 및 제작 기간
- 3인
- 50시간

### 🖥 사용 기술 / 툴
- HTML5
- CSS3
- JavaScript
- VSCode
- Figma

---

## 🧑‍🤝‍🧑 팀원 역할 분담

| 이름 | 주요 작업 | 연락처 |
|------|-----------|-----------|
| **이 봄** (팀장) | 헤더/푸터, 메인 비주얼 슬라이드, 선수 프로필 페이지, 구단 연혁 페이지 | bxrntxdxx@naver.com |
| **김소희** | 메인 1, 3섹션, 선수 목록 페이지, 공지사항 페이지(갤러리) | thsu858585@naver.com |
| **장현민** | 메인 2, 4섹션, 경기 일정 페이지, 공지사항 페이지(목록) | jhm4591@naver.com |

---

## 🌐 배포 링크  
🔗 https://n8220112.github.io/camelcase-fcseoul

### 도메인 구성
```
💾 camelcase-fcseoul/
├── 📑 index.html
├── 📑 members.html
├── 📑 schedule.html
├── 📑 profile.html
├── 📑 history.html
├── 📑 notice.html
├── 📄 header.html / footer.html
├── 📂 css/
│ ├── reset.css
│ ├── variables.css
│ ├── style.css
│ ├── stylesub.css
│ └── general.css
├── 📂 js/
│ ├── custom.js
│ ├── customsub.js
│ └── swiper.js
└── 📂 images/
```

---

## 📷 관련 문서

- **기획서**: [Figma Slides](https://www.figma.com/slides/mgo5Ms3fR81sEVMTgjBJJl/FC%EC%84%9C%EC%9A%B8-%EB%A6%AC%EB%89%B4%EC%96%BC--%EA%B8%B0%ED%9A%8D%EC%84%9C-?node-id=1-42&t=b6SrriTmVYGcRxzR-1)
- **디자인 시안**: [Figma Design](https://www.figma.com/design/edeRTJ9wCZQQcriQp9ipWM/FC-SEOUL-%EB%A6%AC%EB%89%B4%EC%96%BC--%EC%8A%A4%ED%86%A0%EB%A6%AC%EB%B3%B4%EB%93%9C-?node-id=131-2755&t=IEFCSoxTUYbqMbbS-1)

---
## 🧩 메인페이지(index.html) 기능 설명

![Image](https://github.com/user-attachments/assets/fe7e969d-04f5-44e6-b58e-3051a8c1f582)

### ✅ header / footer
- `fetch()`로 외부 HTML 파일을 불러와 삽입
- `window.onscroll`을 이용해 GNB 드롭 애니메이션 구현

### ✅ 로그인 모달
- 로그인 버튼 클릭 시, 모달 창이 열리고  
  닫기 버튼 또는 바깥 영역을 클릭하면 모달이 닫히는 구조
- `display` 속성을 사용한 방식으로,  
  DOM 이벤트 리스너를 통해 상태를 제어

### ✅ GNB
- 마우스 진입 시 서브메뉴 확장 애니메이션
- 스크롤 위치에 따라 메뉴 스타일 변화

### ✅ 메인 비주얼 슬라이드
- 카운트다운 기능 구현
- 오토플레이 프로그래스 바가 swiper 인덱스와 연동되어 동작

![Image](https://github.com/user-attachments/assets/b69a056a-5fa3-4a30-8788-73f8aff2abbd)

### ✅ 대회 순위
- JavaScript 객체 기반 데이터 생성
- `appendChild()`를 이용해 DOM에 순위 테이블 구성

### ✅ 대회 일정
- 카운트다운 기능 구현
- 지도 API 로 경기창 위치 안내

![Image](https://github.com/user-attachments/assets/995fa6bc-e9a3-4289-9281-36038dd43d19)

### ✅ 선수 소개
- 기본 Swiper 슬라이드 구성
- 포지션별 탭 전환 기능 구현

### ✅ SNS 소개
- Swiper.js 사용
- 스토리 일시정지 / 재생 기능 구현 (토글 버튼)

---

## 📄 서브 페이지 기능 요약

![Image](https://github.com/user-attachments/assets/0bfc71db-afda-477a-be49-369acda63df2)

### 🏃‍♂️ 선수 소개 – `members.html`
- 포지션별 탭 메뉴 구현
- 카드 호버 시 선수 이름 표시

![Image](https://github.com/user-attachments/assets/3980c7d9-0ad9-4362-9b7b-2af18732eee8)

### 🧑‍🏫 선수 프로필 – `profile.html`
- 타임라인 기반 스크롤 인터랙션 구현
- 스크롤이 특정 연도에 도달하면 해당 연도의 텍스트 색상이 강조
- 사용자에게 시간의 흐름을 시각적으로 안내

![Image](https://github.com/user-attachments/assets/939b9516-5266-4aa3-a263-641bab489583)

### 🏟️ 구단 연혁 – `history.html`
- 슬라이더와 연동된 수치 및 진행바 애니메이션
- range 타입 슬라이더를 통해 연도를 선택
- 해당 연도의 수상 내역이 숫자와 함께 그래프 형태로 시각화

![Image](https://github.com/user-attachments/assets/a794afaa-dd31-4e67-a004-e6511cbc0479)

### 🗓️ 경기 일정 – `schedule.html`
- 드롭다운으로 연도/월 선택
- 선택된 일정만 표시 (`updateCalendar`)
- 네이버 지도 API 활용 경기장 모달 표시

![Image](https://github.com/user-attachments/assets/6d0a2886-494b-4d92-86a4-8901444d97ec)

![Image](https://github.com/user-attachments/assets/298f76eb-54c9-408e-94da-c4560050d22f)

### 📢 뉴스/공지사항 – `notice.html`
- 뉴스/공지사항 탭 전환 기능
- 페이징 기능 구현
- "더보기" 클릭 시 숨겨진 콘텐츠 노출

---

## ⚠️ 주의사항

- 본 프로젝트는 학습 및 포트폴리오 용도로만 사용됩니다.
- FC서울 구단과는 무관하며, 모든 저작권은 원저작자에게 있습니다.
