<div align="center">

# 🎨 Minseok Choi - Portfolio Website
### 사용자 경험을 최우선으로 생각하는 주니어 프론트엔드 개발자의 포트폴리오

> **"정적인 정보 나열을 넘어, 인터랙티브한 경험을 제공하는 웹사이트"**

<br>

[👉 Live Demo 보러가기 (Click)](https://minseok-portfolio-ochre.vercel.app/)

<br><br>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

</div>

---

## 📖 프로젝트 소개 (Overview)
이 프로젝트는 저의 개발 역량과 경험을 효과적으로 전달하기 위해 기획 및 개발한 **개인 포트폴리오 웹사이트**입니다.
단순히 텍스트 정보를 나열하는 기존의 이력서 방식에서 벗어나, **인터랙티브한 UI 요소**와 **반응형 디자인**을 적용하여 방문자에게 긍정적이고 전문적인 사용자 경험(UX)을 제공하고자 했습니다.

### 🎯 주요 목표
* **접근성 (Accessibility):** PC, 태블릿, 모바일 등 어떤 디바이스에서도 깨지지 않는 최적화된 화면 제공
* **가독성 (Readability):** 기술 스택, 프로젝트 경험 등 핵심 정보가 한눈에 들어오도록 직관적인 레이아웃 설계
* **확장성 (Scalability):** 향후 새로운 프로젝트나 경력이 생겼을 때, 코드를 쉽게 수정하고 업데이트할 수 있는 구조 마련

---

## 🚀 주요 기능 및 특징 (Key Features)

### 1. 🖥️ 반응형 레이아웃 (Responsive Design)
* **Tailwind CSS**의 Breakpoint(`sm`, `md`, `lg`)를 활용하여 디바이스 해상도에 따라 레이아웃이 유연하게 변경됩니다.
* **Desktop:** 프로필과 네비게이션을 왼쪽 사이드바에 고정(Sticky)하여 정보 접근성을 높였습니다.
* **Mobile:** 햄버거 메뉴와 드롭다운 방식을 적용하여 작은 화면에서의 공간 효율성을 극대화했습니다.

### 2. ✨ 인터랙티브 UI (Interactive UI)
* **터미널 로딩 효과:** 개발자의 아이덴티티를 강조하기 위해 첫 화면 진입 시 타자기로 치는 듯한 '터미널 타이핑' 애니메이션을 구현했습니다.
* **스크롤 스파이 (Scroll Spy):** 사용자의 스크롤 위치를 감지하여 현재 보고 있는 섹션의 메뉴가 자동으로 활성화(`active`)됩니다.
* **동적 애니메이션:** `IntersectionObserver`를 활용하여 스킬 숙련도 바가 차오르거나, 요소가 부드럽게 나타나는(Fade-in-up) 효과를 적용했습니다.

### 3. 🛠️ 편의 기능 구현
* **원클릭 복사:** 이메일 아이콘을 클릭하면 주소가 즉시 클립보드에 복사됩니다.
* **PDF 다운로드:** 별도의 페이지 이동 없이 이력서(Resume) 파일을 즉시 다운로드할 수 있습니다.

---

## 💻 기술 스택 (Tech Stack)

| 구분 | 기술 | 설명 |
| :--- | :--- | :--- |
| **Frontend** | ![HTML5](https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white) | 시맨틱 마크업 및 웹 접근성 준수 |
| **Styling** | ![TailwindCSS](https://img.shields.io/badge/-TailwindCSS-38B2AC?logo=tailwind-css&logoColor=white) | 유틸리티 퍼스트 CSS를 활용한 빠른 반응형 UI 개발 |
| **Scripting** | ![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black) | ES6+ 문법 사용, 동적 기능(로딩, 모달, 스크롤 감지) 구현 |
| **Deployment** | ![Vercel](https://img.shields.io/badge/-Vercel-000000?logo=vercel&logoColor=white) | CI/CD 자동화 및 정적 웹사이트 호스팅 |

---

## 📂 디렉토리 구조 (Directory Structure)

```bash
minseok-portfolio
├── index.html             # 메인 페이지 (전체 구조 및 콘텐츠)
├── images/                # 이미지 리소스 폴더
│   ├── me.jpg             # 프로필 사진
│   └── ...                # 프로젝트 썸네일 이미지들
├── minseok_portfolio.pdf  # 포트폴리오 파일
├── minseok_resume.pdf     # 이력서 파일
└── README.md              # 프로젝트 설명 문서
```
---

## 🔧 트러블 슈팅 (Troubleshooting)

### 1. 모바일 환경에서 툴팁 위치 문제
> **문제:** 모바일 화면에서 하단 링크 아이콘을 터치했을 때, 툴팁이 화면 밖으로 잘리거나 다른 요소를 가리는 현상이 발생함.

* **✅ 해결:** CSS Media Query를 활용하여 모바일(`max-width: 768px`) 환경에서는 툴팁을 숨기거나 위치를 강제로 조정했습니다. 또한 PC 환경에서만 `hover` 이벤트가 동작하도록 수정하고, 하단 패딩(`pb-12`)을 충분히 확보하여 UI 간섭을 방지했습니다.

### 2. 스크롤 스파이 성능 최적화
> **문제:** `scroll` 이벤트 리스너를 사용하여 현재 섹션을 감지할 때, 스크롤할 때마다 과도한 이벤트가 발생하여 성능 저하(Reflow) 우려가 있었음.

* **✅ 해결:** `IntersectionObserver API`를 도입했습니다. 브라우저가 뷰포트와 요소의 교차를 비동기적으로 감지하게 함으로써 메인 스레드의 부하를 줄이고, 더 정확하고 부드럽게 섹션 진입을 감지하도록 개선했습니다.

---

## 📞 Contact
* **Email:** minseok.c02@gmail.com
* **GitHub:** [https://github.com/asdzxc000115](https://github.com/asdzxc000115)
