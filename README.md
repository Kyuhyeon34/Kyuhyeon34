<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0B1D2A,35:0E4D64,70:00B4A0,100:7FE7D4&height=140&section=header&text=&fontSize=0" width="100%" alt="Gradient header">

<div align="center">

# 이규현 | Kyuhyeon Lee

**Embedded SW · Linux Driver · Edge AI · FPGA**

MCU 펌웨어와 리눅스 커널 드라이버부터 온디바이스 AI, FPGA 설계까지 하드웨어와 소프트웨어를 잇는 임베디드 개발자입니다.

<a href="mailto:kyuhyeon34@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>

</div>

## 👋 About Me

- 호서대학교 전자공학과 졸업 (2026.02) · 반도체공학 복수전공
- 대한상공회의소 서울기술교육센터 AI 시스템반도체 SW개발자 과정 진행 중
- C 기반 STM32 펌웨어와 Jetson 리눅스 커널 드라이버를 개발하고 있습니다.
- Jetson에서 YOLO 모델을 TensorRT로 변환해 온디바이스 AI 추론을 구현합니다.
- Verilog로 FSM을 설계하고 테스트벤치와 타이밍 분석으로 동작을 검증합니다.

## 🛠 Tech Stack

<h3 align="center">Languages</h3>
<p align="center">
  <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white" alt="C">
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Verilog%20HDL-654FF0?style=for-the-badge" alt="Verilog HDL">
</p>

<h3 align="center">MCU & Boards</h3>
<p align="center">
  <img src="https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white" alt="STM32">
  <img src="https://img.shields.io/badge/Arduino-00878F?style=for-the-badge&logo=arduino&logoColor=white" alt="Arduino">
  <img src="https://img.shields.io/badge/Jetson%20Nano-76B900?style=for-the-badge&logo=nvidia&logoColor=white" alt="Jetson Nano">
</p>

<h3 align="center">Linux Driver & Interfaces</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Linux%20Kernel-333333?style=for-the-badge&logo=linux&logoColor=white" alt="Linux Kernel">
  <img src="https://img.shields.io/badge/Device%20Driver-0E4D64?style=for-the-badge" alt="Device Driver">
  <img src="https://img.shields.io/badge/Device%20Tree-00897B?style=for-the-badge" alt="Device Tree">
  <img src="https://img.shields.io/badge/I2C-0078D4?style=for-the-badge" alt="I2C">
  <img src="https://img.shields.io/badge/UART-0078D4?style=for-the-badge" alt="UART">
  <img src="https://img.shields.io/badge/PWM-0078D4?style=for-the-badge" alt="PWM">
</p>

<h3 align="center">AI & Vision</h3>
<p align="center">
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV">
  <img src="https://img.shields.io/badge/YOLO-111F68?style=for-the-badge" alt="YOLO">
  <img src="https://img.shields.io/badge/TensorRT-76B900?style=for-the-badge&logo=nvidia&logoColor=white" alt="TensorRT">
</p>

<h3 align="center">FPGA & Tools</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Vivado-ED1C24?style=for-the-badge&logo=amd&logoColor=white" alt="Vivado">
  <img src="https://img.shields.io/badge/Basys%203-555555?style=for-the-badge" alt="Basys 3">
  <img src="https://img.shields.io/badge/Qt-41CD52?style=for-the-badge&logo=qt&logoColor=white" alt="Qt">
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git">
</p>

---

## 💻 Projects

### [Curvature Measurement — 레이저 변위센서 기반 비접촉 곡률·평탄도 측정 시스템](https://github.com/Kyuhyeon34/Curvature_Measurement_System)

<img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white" alt="C"> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"> <img src="https://img.shields.io/badge/STM32F411-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32F411"> <img src="https://img.shields.io/badge/ADC-555555?style=flat-square" alt="ADC"> <img src="https://img.shields.io/badge/UART-0078D4?style=flat-square" alt="UART">

- 서보모터로 레이저 변위센서를 -30°~+30° 원호 스캔해 기판의 휨(Bow)과 곡률을 비접촉으로 측정합니다.
- STM32가 30ms 주기로 거리를 샘플링하고, 8회 오버샘플링으로 ADC 분해능을 13.43μm에서 4.75μm로 개선했습니다.
- 세 점 외접원 공식으로 곡률을 계산하고, Python GUI에서 단면 형상과 임계값 0.05mm 초과 지점을 표시합니다.
- 반복 정밀도 0.03mm, 평균 오차율 ±0.03%를 확인했습니다.

### [DC Motor Control — 상태머신 기반 이송 장비 DC 모터 제어 시스템](https://github.com/Kyuhyeon34/DC_Motor_Control)

<img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white" alt="C"> <img src="https://img.shields.io/badge/STM32F411-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32F411"> <img src="https://img.shields.io/badge/PWM-555555?style=flat-square" alt="PWM"> <img src="https://img.shields.io/badge/UART-0078D4?style=flat-square" alt="UART"> <img src="https://img.shields.io/badge/FSM-654FF0?style=flat-square" alt="FSM">

- 버튼 숏클릭·롱클릭과 UART 명령(`F` / `R` / `S`)으로 DC 모터의 정회전·역회전·정지를 제어합니다.
- `STOP` / `FORWARD` / `REVERSE` 상태머신과 이벤트별 함수 포인터 테이블로 입력을 처리합니다.
- 레지스터로 PLL 96MHz 클럭, TIM5 PWM 속도 제어, TIM2 롱클릭 판정, USART2 RX 인터럽트를 설정했습니다.

### [Parking System — 차량 감지 기반 스마트 주차 관제 솔루션](https://github.com/Kyuhyeon34/Parking_System)

<img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++"> <img src="https://img.shields.io/badge/Qt%205-41CD52?style=flat-square&logo=qt&logoColor=white" alt="Qt 5"> <img src="https://img.shields.io/badge/STM32F411-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32F411"> <img src="https://img.shields.io/badge/UART-0078D4?style=flat-square" alt="UART">

- 초음파 센서로 차량을 감지하면 Qt 앱이 입·출차 다이얼로그를 띄우고, 확정 시 STM32가 차단기 모터를 5초 시퀀스로 구동합니다.
- `PING` / `STATE?` / `GATE OPEN` 등 ASCII 시리얼 프로토콜을 설계해 MCU와 PC가 이벤트·거리·상태를 주고받습니다.
- 펌웨어를 `Handler → StateMachine → Controller` 계층으로 나누고, 처리 중에는 초음파 트리거를 멈춰 중복 감지를 막습니다.

### [AI POS System — AI 객체 인식 기반 무인 계산 POS](https://github.com/Kyuhyeon34/AI_POS_System)

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"> <img src="https://img.shields.io/badge/Jetson%20Orin%20Nano-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="Jetson Orin Nano"> <img src="https://img.shields.io/badge/YOLO11-111F68?style=flat-square" alt="YOLO11"> <img src="https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="TensorRT">

- 매대 아래 Jetson이 카메라 영상과 TensorRT 추론 서버를 띄우고, 계산대 PC의 POS가 결과를 받아 주문·결제를 처리합니다.
- YOLO11n 모델 2개를 앙상블하고 좌우 반전 TTA를 더해, 처음 보는 사진 124장에서 mAP50-95 0.977을 얻었습니다.
- POS 안에서 데이터 수집, 자동 라벨링, 재학습, 엔진 변환까지 이어지도록 구성했습니다.

### [Thermal Fan Driver — 커널 드라이버 기반 실시간 온도 감시·냉각 제어](https://github.com/Kyuhyeon34/Thermal_Fan_Driver)

<img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white" alt="C"> <img src="https://img.shields.io/badge/Linux%20Kernel-333333?style=flat-square&logo=linux&logoColor=white" alt="Linux Kernel"> <img src="https://img.shields.io/badge/Device%20Tree-00897B?style=flat-square" alt="Device Tree"> <img src="https://img.shields.io/badge/Jetson%20Orin%20Nano-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="Jetson Orin Nano">

- BMP180(I2C/IIO), DC 모터(PWM), EC11 엔코더(GPIO IRQ), LED 바 커널 드라이버 4종을 Device Tree 오버레이로 연결했습니다.
- 엔코더는 디바운스 타이머와 `kfifo` + `poll`로 회전·클릭·롱프레스 이벤트를 사용자 공간에 전달합니다.
- 사용자 앱은 히스테리시스 기반으로 온도에 따라 팬 듀티를 자동 조절하고, `WAIT` / `AUTO` / `MANUAL` 모드를 전환합니다.

### [FPGA Timer IP — FSM 기반 하드웨어 타이머 IP RTL 설계 및 FPGA 구현](https://github.com/Kyuhyeon34/FPGA_Timer_IP)

<img src="https://img.shields.io/badge/Verilog%20HDL-654FF0?style=flat-square" alt="Verilog HDL"> <img src="https://img.shields.io/badge/Vivado-ED1C24?style=flat-square&logo=amd&logoColor=white" alt="Vivado"> <img src="https://img.shields.io/badge/Basys%203-555555?style=flat-square" alt="Basys 3">

- 분·초 시계와 1/100초 스톱워치 2모드를 FSM으로 설계하고, 4자리 FND를 시분할로 구동합니다.
- 10ms 버튼 디바운서, 틱 생성기, FND 컨트롤러를 모듈로 분리했습니다.
- 테스트벤치 16개 항목 통과, 합성 후 LUT 315 · FF 167, 타이밍 여유 WNS +5.1ns를 확인했습니다.

## 🎓 Education

| 기간 | 소속 / 과정 |
| --- | --- |
| 2020.02 ~ 2026.02 | 호서대학교 전자공학과 졸업 (반도체공학 복수전공) |
| 2026.05 ~ 2026.12 | 대한상공회의소 서울기술교육센터 AI 시스템반도체 SW개발자 과정 (진행 중) |

## 🏆 Awards & Certifications

- **2025 호서대학교 반도체 역량강화 성과발표회 대상**
- **2025 호서대학교 융합교육 학습경험 우수사례 공모전 장려상**
- **TOEIC Speaking IH**

## 📫 Contact

- **Email**: [kyuhyeon34@gmail.com](mailto:kyuhyeon34@gmail.com)

---

<details>
<summary><b>📊 GitHub Activity</b></summary>

<br>

<p align="center">
  <a href="https://github.com/Kyuhyeon34">
    <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=Kyuhyeon34&layout=compact&theme=material-palenight&hide_border=true&bg_color=0B1D2A&text_color=ffffff&title_color=00B4A0" width="40%" alt="Most used languages">
    <img src="https://github-stats-extended.vercel.app/api?username=Kyuhyeon34&show_icons=true&theme=material-palenight&hide_border=true&bg_color=0B1D2A&icon_color=00B4A0&text_color=ffffff&title_color=00B4A0" width="56%" alt="GitHub stats">
  </a>
</p>

<p align="center">
  <img src="https://ghchart.rshah.org/00B4A0/Kyuhyeon34" width="98%" alt="GitHub contribution activity">
</p>

</details>

<br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0B1D2A,35:0E4D64,70:00B4A0,100:7FE7D4&height=40&section=footer&text=&fontSize=0" width="100%" alt="Gradient footer">
