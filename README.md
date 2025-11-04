<div align=center>
<img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=150&section=header&text=Dohee's%20GitHub&fontSize=42" />

<h3>안녕하세요 이도희입니다 <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Slightly%20Smiling%20Face.png" alt="Slightly Smiling Face" width="25" height="25" />
</h3>

📚 Languages / Library / Tools 📚

![js](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![js](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![js](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![js](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![js](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)

</div>
<br>

### 👤 인적사항
- 이름: 이도희
- 전공: 산업보안학과
- 연락처: 010-XXXX-XXXX
- 이메일: dohee050101 [at] gmail [dot] com
- GitHub 주소: https://github.com/dhhi0101
- Notion: [Click here](https://dhhi0101.notion.site/29d16a53543580c39cfbd16d75b942f3?source=copy_link)

<br>

## 🛠 기술 스택

### 🔹 Languages
- **Python**: 기초 문법, 리스트/딕셔너리 활용, 간단한 알고리즘 문제 해결 경험
- **C**: 포인터, 동적 메모리, 파일 입출력 기초 / 멀티스레드 실습 경험
- **Java**: 기본 문법, 클래스/상속/다형성 등 OOP 개념 학습, Swing으로 간단한 GUI 작성

### 🔹 OS & Tools
- **Ubuntu**: ls, cd, mkdir, grep, gcc 등 CLI 기본 명령어 사용
- **VSCode**: 코드 작성, 터미널 실행, Breakpoint 디버깅 활용


<br>

## 📁 프로젝트 경험
### 1️⃣ PQC: Kyber 논문 기반 NTT 연산 구현
**📌 진행 기간:** 2024년 8월  

**📄 내용:** 
- **Crystal-Kyber** 논문[(NIST FIPS 203)](https://share.google/ph9xPsKTtQfnOfF3l) 의 핵심 연산인 `NTT(Number-Theoretic Trasnform)`를 Python으로 구현하여 PQC 계산 흐름 학습

**⚙️ 주요 구현:** NTT / inverse NTT / poly operations

**💡 배운 점:**
- 암호학 논문 기반 알고리즘을 **실제 코드로 구현하는 과정** 경험
- PQC 표준 알고리즘에서 NTT가 **어떤 원리로 동작하는지 학습**

**🔗[GitHub](https://github.com/dhhi0101/kyber-ntt-python)**

<br>

### 2️⃣ C 기반 간단한 랜섬웨어 구현
**📌 진행 기간:** 2024년 2학기

**📄 내용:** 
- `pthread`로 스레드를 분리하여 `target` 디렉터리 내 파일 암호화/복호화하는 시뮬레이터 제작
- XOR 및 AES 방식을 이용해 파일의 헤더 일부만 암호화

**⚙️ 주요 구현:** pthread / mutex sync / XOR / AES

**💡 배운 점:**
- `pthread`를 활용한 멀티스레드 기반 흐름 제어와 `mutex`를 이용한 동기화
- 파일 **헤더 일부만 암호화**하는 실제 랜섬웨어의 효율적인 동작 원리 이해
- C 환경에서 OpenSSL 라이브러리 사용해 **AES API** 호출 경험

**🔗[GitHub](https://github.com/dhhi0101/os-project)**

<br>

### 3️⃣ 라즈베리파이 기반 거리 감지 텔레그램 봇
**📌 진행 기간:** 2025년 1학기

**📄 내용:** 
- 초음파 센서로 실시간 거리 측정하고 30cm 이하 접근 시 LED 점등 및 사진 촬영 후 Telegram으로 알림 전송
- `/start`, `/stop` 명령을 통한 모니터링 제어 기능 구현

**⚙️ 주요 구현:** RPI.GPIO / OpenCV / Telegram bot / threading

**💡 배운 점:**
- 라즈베리파이에서 Python을 활용한 **하드웨어 제어** 경험
- Telegram Bot API, OpenCV 등 다양한 라이브러리 연동
- 실시간 이벤트 기반의 **다중 스레드 동작 구조** 설계 

**🔗[GitHub](https://github.com/dhhi0101/telegram-distance-notice)**

<br>

### 4️⃣ Python 날씨 API + todo list 프로그램
**📌 진행 기간:** 2023년 2학기

**🔧기술 스택:** `Python`, `tkinter`, `requests`, `pandas`

**📄 내용:** 
- `tkinter` GUI 환경에서 `OpenWeatherMap API`를 연동한 오늘의 날씨 조회, Todo List 관리 기능을 하나의 프로그램에 통합

**⚙️ 주요 구현:** 
- `requests`로 OpenWeatherMap API 호출, `json` 파싱한 데이터를 pandas DataFrame으로 변환하여 **오늘 날씨만 필터링**
- `tkinter`의 `Frame`, `Entry`, `Listbox`, `Button` 등 다양한 위젯을 사용해 인터페이스 구축
- 할 일(task)과 마감일(deadline)을 리스트에 저장
- `lambda` 함수를 `sort`의 `key`로 사용하여 자동 정렬

**💡 배운 점:**
- `tkinter` GUI 요소 활용
- API 연동 후 pandas 기반 데이터 처리
- 팀 개발 **협업 경험** (기능별 역할 분담 → 통합)

<br>

### 5️⃣ Java Swing 기반 몬스터 잡기 미니게임
**📌 진행 기간:** 2023년 2학기

**🔧기술 스택:** `Java`, `Java Swing (GUI)`

**📄 내용:** 
- 창 내부를 랜덤으로 이동하는 몬스터 클릭하면 체력 감소
- 체력 0이 되면 제거하고 카운트

**⚙️ 주요 구현:** 
- `Monster`라는 **추상 클래스**를 정의하고 `AttackMonster`와 `DefenseMonster`로 상속 구현
- 몬스터 객체마다 **개별 스레드** 부여, 모든 몬스터가 **동시에 독립적으로** 랜덤하게 움직이도록 구현

**💡 배운 점:**
- 객체지향(OOP) 핵심 개념: **추상화, 상속, 다형성**
- **멀티스레드**를 활용하여 여러 객체가 동시에 동작하는 객체지향 애플리케이션을 설계하는 경험

<br>

### 🌱 자기소개 및 학습 목표
안녕하세요. **'만들면서 배우는' 과정을 통해 성장**하려는 이도희입니다.

PQC 암호학, C언어 멀티스레딩, 라즈베리파이 하드웨어 제어 등 복잡해 보이는 주제도 **일단 부딪혀보고 코드를 작성**하며 이해하려고 노력합니다.

이 리포지토리는 제가 배우기 위해 만들었던 **'작은 실험들'** 의 기록입니다.  

지금의 경험을 바탕으로, 앞으로는 더 견고하고 안전한 시스템을 설계하는 '보안 엔지니어'로 성장하는 것이 목표입니다.
