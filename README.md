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
- 연락처: 010-9619-XXXX
- 이메일: dohee050101@gmail.com
- GitHub 주소: https://github.com/dhhi0101
- Notion: [Click here](https://dhhi0101.notion.site/29d16a53543580c39cfbd16d75b942f3?source=copy_link)

<br>

### 📚 기술스택
**Python**
* 기본 문법 학습, 알고리즘 문제 해결 연습에 사용
  
**C**
* 포인터와 메모리 관리 기본 개념 학습함

**Java**
* 기본 문법과 OOP(클래스, 상속, 다형성 등) 개념 학습함

**Ubuntu**
* 'ls', 'cd', 'mkdir', 'grep', 'gcc' 등 터미널(CLI) 환경의 기본 명령어 사용 익숙

**Visual Studio code (VSCode)**
* 주력 코드 에디터로 사용
* 코드 작성, 터미널 실행, 기본적인 디버깅(Breakpoint) 기능 활용

<br>

### 📁 프로젝트 경험
#### 1️⃣ PQC: Kyber 논문 기반 NTT 연산 구현
**진행 기간:** 2024년 8월

**설명:** 
- 양자내성암호(PQC) 표준 알고리즘 중 하나인 **Crystal-Kyber** 논문[(NIST FIPS 203)](https://share.google/ph9xPsKTtQfnOfF3l) 을 기반으로, 핵심 연산인 `NTT(Number-Theoretic Trasnform)`를 파이썬으로 구현함
- Dilithium 알고리즘의 파이썬 코드를 분석하여 PQC 내부 동작 원리 학습

**사용한 기술:** `Python`

**주요 구현:** 
- Kyber 논문 참고하여 **NTT 및 역NTT 연산** 구현
- NTT를 활용한 **다항식 덧셈 및 곱셈 연산** 구현

**배운 점:**
- 암호학 논문에 기술된 복잡한 수학적 알고리즘(NTT)을 **실제 코드로 옮겨보는 과정**을 경험함
- PQC 표준 알고리즘의 핵심 연산이 **어떤 원리로 동작하는지 학습**하고, 그 구현의 **어려움을 체감**할 수 있었음
- Dilithium 파이썬 코드 분석을 통해 실제 표준 알고리즘이 **어떻게 구조화되어 있는지** 접해볼 수 있었음


**[GitHub 리포지토리 (구현 코드 보기)](https://github.com/dhhi0101/kyber-ntt-python)**

<br>

#### 2️⃣ 간단한 랜섬웨어 구현
**진행 기간:** 2024년 2학기

**설명:**
- `pthread`를 이용해 두 개의 스레드가 동시에 `target` 디렉터리 내의 `.pdf`와 `.jpg` 파일을 탐색하고 암호화/복호화하는 C언어 기반 랜섬웨어 시뮬레이터

**사용한 기술:** `C`, `OpenSSL`

**주요 구현:**
- **하이브리드 방식 암호화:** 파일의 첫 16바이트를 랜덤 마스크와 `XOR` 연산하여 암호화, 이 `mask`를 `AES-128-ECB`로 암호화하여 파일 끝에 덧붙임
- **스레드 동기화:** `pthread_mutex_t`를 사용해 여러 스레드가 공유 자원에 동시에 접근할 때 발생하는 `Race Condition`을 방지하고 동기화 처리

**배운 점:**
- `pthread`를 활용한 멀티스레딩 프로그래밍과 `mutex`를 이용한 **임계 구역 제어** 및 동기화 방법 학습
- 파일 전체가 아닌 헤더(첫 16바이트)만 암호화하고, 암호화에 사용된 키(마스크)를 파일 내에 덧붙이는 실제 랜섬웨어의 **효율적인 동작 원리**를 이해
- OpenSSL 라이브러리를 C언어에서 직접 사용하여 **AES 암호화/복호화 API**를 다루는 경험을 쌓음

**[GitHub 리포지토리 (구현 코드 보기)](https://github.com/dhhi0101/os-project)**

<br>

#### 3️⃣ 라즈베리파이 기반 거리 감지 텔레그램 봇 개발
**진행기간:** 2025년 1학기

**설명:**
- 라즈베리파이에 연결된 **초음파 센서(`HC-SR04`)**로 실시간 거리를 측정
- 사용자가 텔레그램 `/start` 명령으로 모니터링 활성화하면, 거리가 기준(30cm) 이하로 가까워질 시 **USB 카메라**로 사진을 캡처하고 **LED**를 점등시키며 텔레그램으로 경고 메시지와 사진 전송

**사용한 기술:** `Python`, `Raspberry Pi (GPIO)`, `python-telegram-bot`, `OpenCV (cv2)`, `threading`

**주요 구현:**
- **하드웨어 제어 및 API 연동:** `RPI.GPIO`로 초음파 센서/LED 제어, `OpenCV`로 카메라 캡처, `python-telegram-bot` 라이브러리로 `/start`, `/stop` 등 명령어 구현
- **멀티스레딩 아키텍처:** Telegram 봇(메인 스레드)과 별도로, `threading.Thread` 생성하여 **백그라운드 센서 모니터링 루프**가 동기적으로 작동하도록 구현

**배운 점:**
- 라즈베리파이에서 Python을 이용해 `GPIO` 핀을 직접 제어하고, `OpenCV`, `Telegram Bot API` 등 **다양한 하드웨어와 API를 통합**하여 실제 서비스를 구현하는 경험
- 텔레그램 봇의 **비동기(Async) 루프와 동기(Sync) 방식의 실시간 센서 스레드**를 `threading`으로 분리하고, 두 환경을 연동하는 **복잡한 동시성 관리** 방법을 학습

**[GitHub 리포지토리 (구현 코드 보기)](https://github.com/dhhi0101/telegram-distance-notice)**

<br>

#### 4️⃣ Python 날씨 API + todo list 프로그램
> Python 팀 프로젝트로 간단한 프로그램 개발

**진행 기간:** 2023년 2학기

**설명:**
- `tkinter`를 사용해 만든 GUI 애플리케이션으로, `OpenWeatherMap API`를 연동한 '오늘의 날씨' 조회 기능과 '할 일 목록(Todo List)' 관리 기능을 하나의 프로그램에 통합

**사용한 기술:** `Python`, `tkinter`, `requests`, `pandas`

**주요 구현:**
- **API 연동 및 데이터 처리:** `requests`로 OpenWeatherMap API를 호출, `json`으로 파싱한 데이터를 pandas DataFrame으로 변환하여 **오늘 날씨만 필터링**
- **GUI 애플리케이션:** `tkinter`의 `Frame`, `Entry`, `Listbox`, `Button` 등 다양한 위젯을 사용해 날씨 조회 및 할 일 관리 인터페이스 구축
- **데이터 관리 및 정렬:** 할 일(task)과 마감일(deadline)을 리스트에 저장, `lambda` 함수를 `sort`의 `key`로 사용하여 마감일 순서대로 목록을 자동 정렬

**배운 점:**
- `tkinter` GUI 구현과 `requests`/`pandas` API 연동 등 **기능별로 역할을 분담**하고, 각자 개발한 코드를 **하나의 애플리케이션으로 통합**하는 **협업 과정**을 경험

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
