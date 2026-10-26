<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0B1D2A,50:0E4D64,100:00B4A0&height=200&section=header&text=LEE%20KYUHYEON&fontSize=50&fontColor=E6FFFA&fontAlignY=42&desc=Embedded%20SW%20%C2%B7%20Linux%20Driver%20%C2%B7%20Edge%20AI%20%C2%B7%20FPGA&descSize=18&descAlignY=62&animation=fadeIn" width="100%" alt="Header">

<div align="center">

<a href="mailto:kyuhyeon34@gmail.com"><img src="https://img.shields.io/badge/kyuhyeon34@gmail.com-0E4D64?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
<a href="https://github.com/Kyuhyeon34"><img src="https://img.shields.io/badge/GitHub-Kyuhyeon34-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"></a>

</div>

## About Me

**하드웨어와 소프트웨어를 잇는 임베디드 SW 개발자 이규현입니다.**
MCU 펌웨어부터 리눅스 커널 드라이버, 엣지 AI, FPGA 설계까지 직접 만들고 검증해 왔습니다.

- 🎓 호서대학교 전자공학과 · 반도체공학 복수전공
- 💻 대한상공회의소 서울기술교육센터 AI 시스템반도체 SW개발자 과정

## Tech Stack

| 분야 | 기술 |
| --- | --- |
| **Language** | C · C++ · Python · Verilog |
| **MCU** | STM32 (HAL / 레지스터), Arduino |
| **Linux** | Kernel Module, Device Driver, Device Tree |
| **Edge AI** | Jetson, OpenCV, YOLO, TensorRT |
| **FPGA** | Verilog, Vivado, Basys3 |
| **App** | Qt, PyQt |

## Projects

| # | 프로젝트 | 기술 |
| :---: | --- | --- |
| 1 | [**레이저 변위센서 기반 비접촉 곡률·평탄도 측정 시스템 개발**](https://github.com/Kyuhyeon34/Curvature_Measurement_System) | C, Python, STM32, ADC·UART |
| 2 | [**상태머신 기반 이송 장비 DC 모터 제어 시스템 구현**](https://github.com/Kyuhyeon34/DC_Motor_Control) | C, STM32, PWM·UART |
| 3 | [**차량 감지 기반 스마트 주차 관제 솔루션 개발**](https://github.com/Kyuhyeon34/Parking_System) | C/C++, STM32, Qt, UART |
| 4 | [**AI 객체 인식 기반 무인 계산 POS 개발**](https://github.com/Kyuhyeon34/AI_POS_System) | Python, Jetson, YOLO, TensorRT |
| 5 | [**커널 드라이버 기반 실시간 온도 감시·냉각 제어 구현**](https://github.com/Kyuhyeon34/Thermal_Fan_Driver) | Linux Kernel, Device Driver |
| 6 | [**FSM 기반 하드웨어 타이머 IP RTL 설계 및 FPGA 구현**](https://github.com/Kyuhyeon34/FPGA_Timer_IP) | Verilog, Vivado, Basys3 |

### 1. 레이저 변위센서 기반 비접촉 곡률·평탄도 측정 시스템
- 서보모터로 레이저 변위센서를 -30°~+30° 원호 스캔해 기판의 휨(Bow)과 곡률을 비접촉 측정
- STM32에서 30ms 주기 샘플링, 8회 오버샘플링으로 분해능 13.43μm → 4.75μm 개선
- Python GUI로 단면 형상 실시간 시각화, 임계값 0.05mm 초과 시 불량 자동 판정 · 반복 정밀도 0.03mm

### 2. 상태머신 기반 이송 장비 DC 모터 제어 시스템
- 버튼 숏·롱클릭과 UART 명령으로 정회전·역회전·정지를 제어하는 `STOP / FORWARD / REVERSE` 상태머신
- 레지스터 직접 설정으로 PLL 96MHz 클럭, TIM5 PWM 속도 제어, TIM2 롱클릭 판정 구현

### 3. 차량 감지 기반 스마트 주차 관제 솔루션
- 초음파로 차량을 감지하면 Qt 앱이 입·출차를 처리하고 STM32가 차단기 모터를 제어
- MCU–PC 간 ASCII 시리얼 프로토콜 설계, `Handler → StateMachine → Controller` 계층 구조

### 4. AI 객체 인식 기반 무인 계산 POS
- Jetson에서 YOLO11n을 TensorRT로 추론하고 PC POS가 결과를 받아 주문·결제 처리
- 모델 2개 앙상블 + TTA로 처음 보는 사진 124장 기준 mAP50-95 0.977

### 5. 커널 드라이버 기반 실시간 온도 감시·냉각 제어
- Jetson Orin Nano에서 BMP180(I2C/IIO), DC 모터(PWM), 엔코더(IRQ), LED 바 커널 드라이버 4종 개발
- 히스테리시스 기반 온도-팬 속도 자동 제어 앱 (`WAIT / AUTO / MANUAL`)

### 6. FSM 기반 하드웨어 타이머 IP RTL 설계 및 FPGA 구현
- 시계·스톱워치 2모드 FSM, 버튼 디바운서, FND 시분할 구동을 Verilog 모듈로 설계
- 테스트벤치 16개 항목 통과, 합성 후 타이밍 여유 WNS +5.1ns 확인

## Awards & Certifications

| 이름 | 기관 | 날짜 |
| --- | --- | :---: |
| 반도체 역량강화 성과발표회 대상 | 호서대학교 | 2025.12 |
| 융합교육 학습경험 우수사례 공모전 장려상 | 호서대학교 | 2025.12 |
| TOEIC Speaking IH | ETS | 2026.10 |

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00B4A0,50:0E4D64,100:0B1D2A&height=100&section=footer" width="100%" alt="Footer">
