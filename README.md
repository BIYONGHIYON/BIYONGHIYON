<h1 align="center">동국대학교 멀티미디어공학과 이병현</h1>

<p align="center">
  <a href="https://biyonghiyon.github.io/portfolio/">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=githubpages&logoColor=white" alt="Portfolio" />
  </a>
</p>

---

## 🧗 대표 프로젝트

<div align="center">
  <img
    width="130"
    height="130"
    alt="TopOut 로고"
    src="https://github.com/user-attachments/assets/f3f75e67-414c-4a6a-92f2-52b47f9badbd"
  />

  <h3>TopOut</h3>

  <strong>등반 시작부터 완등 순간까지, 자동으로 찾아주는 클라이밍 촬영 앱</strong>
</div>

<br />

TopOut은 사용자의 움직임을 기기 안에서 분석해 등반 구간을 자동으로 찾아주는 iOS·Android 앱입니다.

- iOS와 Android 앱 직접 개발 및 출시
- 움직임·자세·매트 경계를 활용한 온디바이스 영상 분석
- 카메라 촬영부터 구간 탐지, 정밀 편집, 갤러리 저장까지 구현
- 저사양 기기, 메모리, 발열, 배터리 및 촬영 중단 상황 대응
- 9개 언어 지원 및 실제 사용자 피드백을 기반으로 기능과 사용 흐름 개선
- 회원가입 없이 사용하며 영상 분석은 기기 안에서 수행

### 🍎 iOS

<p>
  <img src="https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white" alt="Swift" />
  <img src="https://img.shields.io/badge/UIKit-2396F3?style=flat-square&logo=apple&logoColor=white" alt="UIKit" />
  <img src="https://img.shields.io/badge/AVFoundation-000000?style=flat-square&logo=apple&logoColor=white" alt="AVFoundation" />
  <img src="https://img.shields.io/badge/Vision-5E5CE6?style=flat-square&logo=apple&logoColor=white" alt="Vision" />
  <img src="https://img.shields.io/badge/Core_ML-147EFB?style=flat-square&logo=apple&logoColor=white" alt="Core ML" />
</p>

### 🤖 Android

<p>
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose" />
  <img src="https://img.shields.io/badge/CameraX-3DDC84?style=flat-square&logo=android&logoColor=white" alt="CameraX" />
  <img src="https://img.shields.io/badge/LiteRT-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" alt="LiteRT" />
  <img src="https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square&logo=onnx&logoColor=white" alt="ONNX Runtime" />
</p>

### 🔗 TopOut 바로가기

<p>
  <a href="https://github.com/BIYONGHIYON/TopOut-app">
    <img src="https://img.shields.io/badge/프로젝트_소개-181717?style=for-the-badge&logo=github&logoColor=white" alt="프로젝트 소개" />
  </a>
  <a href="https://apps.apple.com/kr/app/topout/id6790163178">
    <img src="https://img.shields.io/badge/App_Store-0D96F6?style=for-the-badge&logo=appstore&logoColor=white" alt="App Store" />
  </a>
  <a href="https://play.google.com/store/apps/details?id=com.topout.cam">
    <img src="https://img.shields.io/badge/Google_Play-414141?style=for-the-badge&logo=googleplay&logoColor=white" alt="Google Play" />
  </a>
</p>

<p>
  <a href="https://topout-portfolio.vercel.app/">
    <img src="https://img.shields.io/badge/TopOut_Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="TopOut Portfolio" />
  </a>
  <a href="https://www.instagram.com/topout_app/">
    <img src="https://img.shields.io/badge/@topout__app-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="TopOut Instagram" />
  </a>
</p>

---

## 🛰️ 위성영상 팬샤프닝 연구

### [CtrS](https://github.com/BIYONGHIYON/CtrS)

고해상도 흑백 위성영상(PAN)의 공간 정보와 저해상도 다중분광영상(MS)의 색·분광 정보를 결합해 고해상도 MS를 복원하는 팬샤프닝 연구입니다. 동국대학교 종합설계1 CtrS팀 팀장으로 4명이 함께 SSA-MRN의 성능을 개선하고 있습니다.

- **새 기준 모델 C2MS:** 원본 SSA-MRN에 병렬 가지를 더하고, 원래 학습 쌍과 2배 거친 학습 쌍을 섞어 학습
- **QB 성능:** 원본 대비 RR PSNR +0.87 dB (3시드 평균)
- **다른 센서:** GF2·WV3에서 RR PSNR +2.05·+1.01 dB, 학습하지 않은 WV2에서도 +0.83 dB (3시드 평균)
- **색 정확도:** 학습하지 않은 WV2에서 가장 큰 밴드 밝기 치우침 7.2% → 1.0%

`Python` · `PyTorch` · `Pansharpening` · `Remote Sensing`

![WV2 결과 예시: LR MS · PAN · 원본 SSA-MRN · C2MS · 정답](https://raw.githubusercontent.com/BIYONGHIYON/CtrS/main/SSA-MRN/experiments/performance/54_multi_sensor_scale_mixed_training/results/images/WV2_C2MS_vs_original/full_scene_00.png)

위 줄 왼쪽부터 **LR MS · PAN 입력 · 원본 SSA-MRN · C2MS · 정답**, 아래 줄은 원본과 C2MS의 오차 지도입니다(밝을수록 오차가 큼). WV3로 학습한 모델을 학습하지 않은 WV2 장면에 적용한 결과입니다.

[연구 코드·실험 결과](https://github.com/BIYONGHIYON/CtrS)

---

## 🛠️ 다른 프로젝트

### 📡 [Linkcast](https://github.com/BIYONGHIYON/linkcast)

USB 캡처보드나 화면 공유로 입력한 콘솔·PC 화면을 링크 하나로 공유하는 **소규모 실시간 방송 서비스**입니다. 송출자가 최대 5명에게 영상을 보내고, 모두가 브라우저에서 음성으로 대화할 수 있습니다.

- **초저지연 송출:** WebRTC P2P로 최대 1080p 60fps 영상 전송
- **음성 통화:** 송출자와 참가자 전원이 브라우저에서 대화
- **레이저 모드:** 클릭·터치 드래그로 화면 위 포인터 공유
- **다양한 입력:** USB 캡처보드, 프로그램 창·전체 화면·브라우저 탭 공유
- **시그널링:** Cloudflare Workers · Durable Objects로 방 입장과 연결 관리

`TypeScript` · `React` · `WebRTC` · `Cloudflare Workers`

[서비스 열기](https://linkcast.byeonghyeon383.workers.dev/) · [소스 코드](https://github.com/BIYONGHIYON/linkcast)

---

### 🚀 [NODE](https://github.com/BIYONGHIYON/NODE)

두 우주비행사가 로프를 이용해 우주를 탐험하는 **2인 로컬 협동 퍼즐 플랫폼 게임**입니다. Unity와 C#으로 개발했으며, 두 플레이어가 움직임과 로프를 조합해 장애물을 넘고 퍼즐을 해결합니다.

- **로프 액션:** 파트너나 지형에 로프를 걸고 스윙하며 이동
- **행성별 중력:** 무중력·저중력 환경에 따라 달라지는 이동과 퍼즐
- **협동 퍼즐:** 운석과 지형지물을 밀고 당기며 연료통 수집
- **탐험과 진행:** 체크포인트를 통과하고 연료를 모아 다음 행성으로 이동
- **PC 배포:** Windows·macOS 실행 파일 제공

`Unity 2022` · `C#` · `2.5D` · `Local Co-op`

https://github.com/user-attachments/assets/5ab698a2-caba-4773-ac90-e37cc6a2ec21

[소스 코드·조작 안내](https://github.com/BIYONGHIYON/NODE) · [다운로드](https://github.com/BIYONGHIYON/NODE/releases/latest)

---

## 🔍 관심 분야

<p>
  <img src="https://img.shields.io/badge/Computer_Vision-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="Computer Vision" />
  <img src="https://img.shields.io/badge/Camera-111111?style=flat-square&logo=camera&logoColor=white" alt="Camera" />
  <img src="https://img.shields.io/badge/Video_Processing-FF0000?style=flat-square&logo=youtube&logoColor=white" alt="Video Processing" />
  <img src="https://img.shields.io/badge/On--device_AI-412991?style=flat-square&logo=openai&logoColor=white" alt="On-device AI" />
</p>

컴퓨터 비전 · 카메라 및 영상 처리 · 온디바이스 분석 · Multimodal 영상 융합
