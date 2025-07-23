# 💸 Spending Diary

**Python + CustomTkinter 기반의 GUI 가계부 프로그램**입니다.  
날짜별 수입/지출 기록을 입력하고, 막대그래프 형태로 통계를 시각화할 수 있습니다.  
파일 저장은 CSV 기반으로 처리하며, 깔끔한 인터페이스를 갖춘 데스크탑용 프로그램입니다.

---

## 🗓️ 개발 기간
**2025년 1월 25일 ~ 2월 10일**

## 👤 프로젝트 형태
**개인 프로젝트**

## 📝 주제 선정 이유
어렸을 때부터 용돈 기입장을 쓰는 습관이 있었고,  
이를 바탕으로 나만의 가계부 프로그램을 만들어보고 싶었습니다.

---

## 🎯 프로젝트 개요

- Python으로 만든 **GUI 기반 가계부 앱**
- 날짜, 카테고리, 금액, 메모 입력 후 **CSV 저장**
- **막대 그래프를 통한 시각화**로 지출 현황 확인
- CustomTkinter를 활용한 직관적 UI 구현

---

## 💡 주요 기능

- 날짜 클릭 후 수입/지출 항목 등록
- 카테고리, 금액, 메모 입력 기능
- 기록 저장 및 불러오기 (CSV 파일 기반)
- **matplotlib**을 활용한 지출 통계 시각화

---

## 📦 활용 패키지

| 패키지 | 설명 |
|--------|------|
| `customtkinter` | GUI 구성 (Tkinter 확장) |
| `tkinter` | 기본 GUI 구성 |
| `matplotlib` | 통계 그래프 시각화 |
| `csv` | 파일 입출력 처리 |
| `datetime` | 날짜 계산 및 형식 처리 |

---

## 📁 프로젝트 구조
```
SpendingDiary/
├── Spending_diary.py # 메인 실행 파일 (진입점)
├── main_screen.py # 메인 화면 UI 구성
├── ui_manager.py # GUI 요소 관리
├── theme.py # 색상 테마 설정
├── file_manager.py # 파일 입출력 처리
├── record_manager.py # 기록 저장 및 조회
├── date_utils.py # 날짜 계산 유틸 함수
├── func_manager.py # 기능 핸들링 (등록, 삭제 등)
├── records.csv # 기록 저장용 CSV 파일
├── pycache/ # 파이썬 캐시 폴더 (자동 생성)
└── .vscode/ # VSCode 환경 설정 (자동 생성)
```

---

## 🧩 기술 포인트

- `CustomTkinter`로 구성한 직관적인 GUI
- `calendar` 위젯 활용 달력 기능 구현
- `matplotlib`로 카테고리별 지출 통계 시각화
- 파일 단위 기능 모듈화 → 유지 보수에 용이한 구조
- 날짜 처리, 시각화, 파일 저장 등을 각각의 모듈로 구분하여 효율적인 관리

---

## 📌 프로젝트에서 배운 점

- GUI 구조 설계 및 사용자 인터페이스 구성의 흐름 이해
- 기능 단위로 분리하여 코드 구조를 개선하는 경험
- `matplotlib` 기반 시각화 기능 사용 경험
- 파일 단위 모듈화를 통해 **확장성과 유지 보수성 확보**

---

## ✏️ 아쉬웠던 점

- 첫 프로젝트라 Git 브랜치 관리가 미흡했던 점
- 날짜 형식 불일치로 에러가 발생 → 날짜 처리 유틸 함수로 해결
- `pandas`나 `numpy`를 배우기 전이라 데이터 처리를 딕셔너리 위주로만 구현한 점
- **파이 차트 등 다양한 시각화 방법**을 추가해보지 못한 점

---

## 🔗 관련 링크

- 📂 GitHub Repository: [https://github.com/sua-repo/spending-diary.git](https://github.com/sua-repo/spending-diary.git)  
- 📝 발표 자료 (PDF): [발표자료 보기](https://drive.google.com/file/d/1kiPCuj4XuML2g6M-4jFJtthR5U1m95Dc/view?usp=drive_link)  
- 📄 프로젝트 소개 Notion 페이지: [프로젝트 정리 바로가기](https://www.notion.so/Spending-Diary-238f8c4af4728099b70cf027e9e0cdb3)

---

## ▶️ 실행 방법

### 1. 패키지 설치
```bash
pip install customtkinter matplotlib
```

### 2. 실행
python Spending_diary.py
💡 Spending_diary.py는 전체 프로그램의 진입점입니다. 창을 생성하고 메인 화면을 호출합니다.
