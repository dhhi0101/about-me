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
