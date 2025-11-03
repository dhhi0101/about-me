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

**🔧 기술 스택:** `Python`

**📄 내용:** 
- 양자내성암호(PQC) 표준 알고리즘 중 하나인 **Crystal-Kyber** 논문[(NIST FIPS 203)](https://share.google/ph9xPsKTtQfnOfF3l) 의 핵심 연산인 `NTT(Number-Theoretic Trasnform)`를 Python으로 구현
- Dilithium 알고리즘의 Python 코드를 분석하여 PQC 내부 동작 원리 학습

**⚙️ 주요 구현:** 
- Kyber 논문 참고 **NTT / 역NTT 연산** 구현
- **다항식 덧셈 및 곱셈 연산** 수행

**💡 배운 점:**
- 암호학 논문을 기반으로 알고리즘을 **실제 코드로 구현하는 과정** 경험
- PQC 표준 알고리즘에서 NTT가 **어떤 원리로 동작하는지 학습**하고, 구현의 **어려움을 체감**함
- Dilithium 분석을 통해 실제 **표준 알고리즘의 구조** 이해


**🔗[GitHub](https://github.com/dhhi0101/kyber-ntt-python)**

<br>

### 2️⃣ C 기반 간단한 랜섬웨어 구현
**📌 진행 기간:** 2024년 2학기

**🔧기술 스택:** `C`, `OpenSSL`, `pthread`

**📄 내용:** 
- `pthread`를 이용해 두 개의 스레드가 동시에 `target` 디렉터리 내의 `.pdf`, `.jpg` 파일을 탐색
- 간단한 암호화/복호화 수행하는 시뮬레이터 구현

**⚙️ 주요 구현:** 
- 파일의 첫 16바이트 → 랜덤 mask과 `XOR` 연산 암호화
- `mask`값 `AES-128-ECB`로 암호화 후 파일 끝에 append
- `pthread_mutex_t`로 여러 스레드가 공유 자원에 동시 접근 시 동기화 처리

**💡 배운 점:**
- `pthread`를 활용한 멀티스레딩 구조와 `mutex`를 이용한 임계 구역 제어
- 파일 **헤더 일부만 암호화**하는 실제 랜섬웨어의 효율적인 동작 원리 이해
- OpenSSL 라이브러리 활용해 **AES API**를 호출해보는 경험

**🔗[GitHub](https://github.com/dhhi0101/os-project)**

<br>

### 3️⃣ 라즈베리파이 기반 거리 감지 텔레그램 봇
**📌 진행 기간:** 2025년 1학기

**🔧기술 스택:** `Python`, `Raspberry Pi (GPIO)`, `python-telegram-bot`, `OpenCV (cv2)`, `threading`

**📄 내용:** 
- 연결된 초음파 센서(`HC-SR04`) 로 실시간 거리 측정
- 30cm 이하 접근 시 사진 촬영 + LED 점등 + Telegram에 알림 발송
- 사용자가 `/start` 입력 시 모니터링 시작, `/stop`시 중단

**⚙️ 주요 구현:** 
- `RPI.GPIO`로 초음파 센서/LED 제어
- `OpenCV`로 USB 카메라 이미지 캡처
- `python-telegram-bot` 라이브러리로 `/start`, `/stop` 등 명령 제어
- 메인 스레드와 센서 모니터링 스레드를 **threading**으로 분리

**💡 배운 점:**
- 라즈베리파이에서 Python을 활용한 **하드웨어 제어** 경험
- Telegram Bot API, OpenCV 등 다양한 라이브러리 연동
- 실시간 이벤트 기반의 **다중 스레드 동작 구조** 설계 및 처리 

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

#### 5️⃣ Java Swing 기반 몬스터 잡기 미니게임
**진행 기간:** 2023년 2학기

**설명:**
- Java `Swing`을 사용해 만든 GUI 게임으로, 몬스터가 창 안에서 랜덤하게 움직임
- 사용자가 몬스터를 마우스로 클릭하면 방어력에 따라 체력이 감소하며, 체력이 0이 되면 몬스터가 사라지고 잡은 몬스터 수가 카운트

**사용한 기술:** `Java`, `Java Swing (GUI)`

**주요 구현:**
- **객체지향 프로그래밍 (OOP):** `Monster`라는 **추상 클래스**를 정의하고, 이를 상속받은 `AttackMonster`와 `DefenseMonster` 클래스를 구현하여 **다형성** 활용
- **멀티스레딩:** 몬스터 객체마다 `MoveThread`를 **개별 스레드**로 생성하여, 모든 몬스터가 **동시에 독립적으로** 랜덤하게 움직이도록 구현

**배운 점:**
- **추상 클래스와 상속**, 그리고 **멀티스레드**를 활용하여 여러 객체가 각자의 로직을 가지고 동시에 동작하는 객체지향 애플리케이션을 설계하는 경험을 함

<br>

### 🌱 자기소개 및 학습 목표
안녕하세요. **'만들면서 배우는' 과정을 통해 성장**하려는 이도희입니다.

PQC 암호학, C언어 멀티스레딩, 라즈베리파이 하드웨어 제어 등 복잡해 보이는 주제도 **일단 부딪혀보고 코드를 작성**하며 이해하려고 노력합니다.

이 리포지토리는 제가 배우기 위해 만들었던 **'작은 실험들'** 의 기록입니다.  

지금의 경험을 바탕으로, 앞으로는 더 견고하고 안전한 시스템을 설계하는 '보안 엔지니어'로 성장하는 것이 목표입니다.
