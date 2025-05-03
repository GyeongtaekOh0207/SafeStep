# 🥾 SafeStep
> ### 신발 마모도 실시간 측정 스테이션

## 📋 프로젝트 소개

**신발 마모도를 실시간으로 측정하여 낙상사고를 예방하고 안전한 보행 환경을 제공하는 AI 기반 솔루션**

- **프로젝트 기간**: 2025.03 ~ 2025.04
- **팀 구성**: 본인 포함 4인 참여

---

## 💡 프로젝트 개요

SafeStep 프로젝트는 일상생활에서 간과되기 쉬운 신발 밑창 마모로 인한 낙상사고를 예방하기 위해 시작되었습니다.

사람들이 신발 밑창의 상태를 제대로 확인하지 않는 문제점에 착안하여, 인공지능과 IoT 기술을 활용해 신발 마모도를 자동으로 측정하고 필요시 미끄럼 방지 처리를 제공하는 시스템을 개발했습니다.

이 프로젝트는 특히 안전 취약계층을 위한 공공 서비스로 활용될 수 있으며, 산업 현장에서의 안전사고 예방에도 기여할 수 있습니다.

---

## 📺 Demo

### 📷 시연 사진

<table>
  <tr>
    <td align="center" width="50%" colspan="2">
      <h4>마모도 50% 테스트 결과</h4>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/dbbd79fc-ffa1-46bb-ac3d-94fe9df77114" width="350px">
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/3600b21e-7086-449c-8c1d-153872fe371a" width="350px">
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>마모도 50% 디스플레이 화면</b>
    </td>
    <td align="center">
      <b>마모도 50% 내부 처리 과정</b>
    </td>
  </tr>

  <tr>
    <td align="center" width="50%" colspan="2">
      <h4>마모도 70% 테스트 결과</h4>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/982b7eea-53b7-48c5-bde0-91fb44f22a77" width="350px">
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/ffb4156f-b606-4681-9f11-1e585de73ef9" width="350px">
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>마모도 70% 디스플레이 화면</b>
    </td>
    <td align="center">
      <b>마모도 70% 내부 처리 과정</b>
    </td>
  </tr>
</table>

### 🎬 시연 영상

<div align="left">
  <a href="https://www.youtube.com/playlist?list=PLRV3YgAS3RKgM1JDzlZSapaO-rVuEehmB" target="_blank">
    <img src="https://img.shields.io/badge/YouTube-SafeStep%20시연%20영상%20보기-red?style=for-the-badge&logo=youtube" alt="SafeStep 시연 영상">
  </a>
</div>

---

## 👥 팀원 소개

<div align="center">

| **오경택(팀장)** | **홍훈의(부팀장)** | **임정환(조원)** | **조정호(조원)** |
| :------: | :------: | :------: | :------: |
| [<img src="https://github.com/user-attachments/assets/4e865b7d-c93f-477d-af75-31c7ac30d4ce" height=150> <br/> gyeongtaek.dev@gmail.com](#) | [<img src="https://github.com/user-attachments/assets/c18a97f8-7f4b-417e-96ff-4cec6845e58b" height=150> <br/> asdfzxcv5621@naver.com](#) | [<img src="https://github.com/user-attachments/assets/5d49bcec-07a8-4437-9647-9d77bcc3fa26" height=150> <br/> halim0214@gmail.com](#) | [<img src="https://github.com/user-attachments/assets/ae84cab1-b0ff-4336-af62-064a971fbf91" height=150> <br/> peenut9708@daum.net](#) |

</div>
<br>

---

## ⚙️ 프로젝트 구성

### 🔧 하드웨어
- **메인 서버**: Raspberry Pi 4
- **AI 처리**: NVIDIA Jetson Nano
- **센서/액추에이터 제어**: Arduino Mega
- **기타 장비**: 카메라 모듈, 서보모터, 로드셀, LED 스트립, IR 센서

### 💻 소프트웨어
- **객체 감지 모델**: YOLOv8
- **이미지 처리**: OpenCV
- **웹 서버**: PHP
- **데이터베이스**: MariaDB

### 🌐 네트워크
- 서버-클라이언트 구조로 TCP/IP 소켓 통신
- NFS 파일 공유 시스템 활용

### 🧠 알고리즘
- 신발 밑창 마모도 분석을 위한 딥러닝 모델
- 4단계 마모도 분류: 정상, 30%, 50%, 70%

### 📊 회로도

![safestep](https://github.com/user-attachments/assets/27c5ccfd-bfd4-4680-99dd-c108100d4db4)

<div align="left">
  <a href="https://drive.google.com/file/d/1JAlKQ0xJ__RQuyoeVCvxJKp7c3nCNwuF/view?usp=sharing" target="_blank">
    <img src="https://img.shields.io/badge/Draw.io-SafeStep%20회로도%20보기-orange?style=for-the-badge&logo=diagramsdotnet" alt="SafeStep 회로도">
  </a>
</div>

---

## 🛠️ 프로젝트 구현

### 👟 신발 감지 시스템
- 로드셀을 통해 신발이 놓였을 때 무게를 감지하고 플래그를 서버로 전송

### 🔍 이미지 처리 파이프라인
- 카메라로 신발 밑창을 촬영하여 Jetson Nano에서 YOLOv8 모델로 분석

### ⚡ 자동 대응 메커니즘
- 마모도에 따라 스프레이 분사 또는 스프레이 보관함 개방 등 단계별 대응

### 👤 사용자 인터페이스
- 웹 기반 대시보드를 통해 마모 상태 및 조치 사항 시각화 제공

---

## 🔑 맡은 역할

- AI 모델 설계 및 훈련
- 데이터셋 구축 및 전처리
- 실시간 처리 최적화
- 시스템 통합 및 테스트
- 통신 시스템 연결

---

## ⚠️ 문제와 문제해결

### 1️⃣ 데이터셋 부재

#### 첫번째 시도: 편집과 그림툴을 이용한 데이터셋 구축
- 찍은 사진 30장으로 800장 데이터셋 생성
- **결과**: 데이터셋이 일관되지 않고 마모도 분류가 제대로 되지 않음

<table>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/2b9f44b9-5ede-4905-956a-a6bec139add5" width="250px"><br>
      <b>50% 마모도 예시</b> (그림툴 활용)
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/f3d9c05d-1fb5-4654-b679-b9875d2fca82" width="250px"><br>
      <b>70% 마모도 예시</b> (그림툴 활용)
    </td>
  </tr>
</table>

#### 두번째 시도: 슬리퍼 4쌍을 인공적으로 마모시켜 데이터셋 구축
- 사진량을 1200장으로 증가
- 여러 각도에서 흰색 배경으로 촬영
- **결과**: 너무 많은 각도에서 촬영하여 신발 일부가 흐려져 높은 마모도로 잘못 인식

#### 세번째 시도: 균일한 환경에서 신발 전체가 명확히 나오도록 변경
- 사진량을 2400장으로 증가
- 빛과 각도를 조절하고 신발 전체가 명확히 나오도록 촬영
- **결과**: 마모도간 인식률 향상 및 구분을 더 명확하게 개선

<table>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/615d22fe-8f62-4c5b-a482-7d6493ed669d" width="250px"><br>
      <b>50% 마모도 예시</b> (인공 마모)
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/d62577e3-4e72-4b76-b879-09d304046630" width="250px"><br>
      <b>70% 마모도 예시</b> (인공 마모)
    </td>
  </tr>
</table>

### 2️⃣ 실시간 처리 최적화

- **초기 시도**: YOLOv8 nano 모델 선택 (처리 속도 12초)
- **문제점**: 인식률이 높지 않음 (인식률 50%)
- **해결책**: YOLOv8 small 모델로 변경하여 속도와 정확도의 균형 확보 (처리 속도 20초, 인식률 80%)
- **향후 개선점**: 다양한 데이터 전처리 단계를 통한 인식률 향상

### 3️⃣ 통신 안정성

- **문제**: 무선 통신 환경에서의 데이터 손실 위험
- **해결책**: 연결 재시도 메커니즘, 연결 상태 확인, 뮤텍스를 활용한 스레드 동기화, 예외 처리를 통한 오류 처리 등등 다양한 방법들을 사용하여 네크워크가 불안한 환경에서도 빠른 시간 내에 복구되어 사용할 수 있도록 해주었습니다.

---

## 🏁 결론

SafeStep 프로젝트는 인공지능과 IoT 기술을 활용하여 일상생활에서 간과되기 쉬운 안전 문제를 해결하는 사례를 제시했습니다.

본 시스템은 공공장소, 산업 현장 등 다양한 환경에서 활용될 수 있으며, 특히 안전 취약계층을 위한 서비스로서 가치가 있습니다.

### 🔮 향후 발전 방향
- 더 다양한 신발 유형에 대한 데이터 확장
- 개인화된 사용자 경험 제공
- 추가 센서를 통한 정밀도 향상

SafeStep은 단순한 기술 구현을 넘어 사회 안전망 구축에 기여하는 의미 있는 프로젝트로 자리매김할 수 있을 것입니다.
