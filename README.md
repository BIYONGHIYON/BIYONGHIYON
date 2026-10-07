<h1 align="center">동국대학교 멀티미디어공학과 이병현</h1>

<p align="center">
  <a href="https://topout-portfolio.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" />
  </a>
  <a href="https://www.instagram.com/topout_app/">
    <img src="https://img.shields.io/badge/TopOut_Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="TopOut Instagram" />
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

## 🔬 RGB–HSI 초해상도 연구

### [RGB-HSI-SR](https://github.com/BIYONGHIYON/RGB-HSI-SR)

고해상도 RGB의 공간 정보를 활용해 저해상도 초분광 영상(HSI)의 해상도를 높이는 연구입니다. SSA-MRN을 기반으로 공간 경계를 복원하면서 각 픽셀의 분광 정보를 유지하는 방법을 실험합니다.

- **204밴드 HSI 복원:** LIB-HSI의 합성 ×4 축소 데이터를 이용해 공간 초해상도 평가
- **구조 비교:** RGB 채널별 분광 특징 추출과 공동 디코더, 23탭 보간 및 LR 평균 일관성 보정
- **손실 함수 실험:** 값의 오차와 스펙트럼 모양, 영상 경계를 함께 고려해 PSNR·SAM 평가
- **결과 공개:** 실험별 수치·그래프·비교 이미지와 204밴드 슬라이더 웹뷰어 제공

합성 축소 평가와 실제 센서 환경의 성능을 구분하고, 동일 조건의 대조군과 비교해 개선 효과를 확인합니다.

`Python` · `PyTorch` · `Hyperspectral Imaging` · `Super-Resolution`

[연구 코드·실험 결과](https://github.com/BIYONGHIYON/RGB-HSI-SR) · [알고리즘 설명](https://github.com/BIYONGHIYON/RGB-HSI-SR/blob/main/SSA-MRN/docs/research.md) · [204밴드 웹뷰어](https://biyonghiyon.github.io/RGB-HSI-SR/ssa-mrn/)

---

## 🛠️ 다른 프로젝트

### 🚀 [NODE](https://github.com/BIYONGHIYON/NODE)

두 우주비행사가 로프를 이용해 우주를 탐험하는 **2인 로컬 협동 퍼즐 플랫폼 게임**입니다. Unity와 C#으로 개발했으며, 두 플레이어가 움직임과 로프를 조합해 장애물을 넘고 퍼즐을 해결합니다.

- **로프 액션:** 파트너나 지형에 로프를 걸고 스윙하며 이동
- **행성별 중력:** 고중력·무중력 환경에 따라 달라지는 이동과 퍼즐
- **협동 퍼즐:** 운석과 지형지물을 밀고 당기며 연료통 수집
- **탐험과 진행:** 체크포인트를 통과하고 연료를 모아 다음 행성으로 이동
- **PC 배포:** Windows·macOS 실행 파일 제공

`Unity 2022` · `C#` · `2.5D` · `Local Co-op`

[소스 코드·조작 안내](https://github.com/BIYONGHIYON/NODE) · [플레이 영상](https://github.com/user-attachments/assets/5ab698a2-caba-4773-ac90-e37cc6a2ec21) · [다운로드](https://github.com/BIYONGHIYON/NODE/releases/latest)

---

## 🔍 관심 분야

<p>
  <img src="https://img.shields.io/badge/Computer_Vision-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="Computer Vision" />
  <img src="https://img.shields.io/badge/Camera-111111?style=flat-square&logo=camera&logoColor=white" alt="Camera" />
  <img src="https://img.shields.io/badge/Video_Processing-FF0000?style=flat-square&logo=youtube&logoColor=white" alt="Video Processing" />
  <img src="https://img.shields.io/badge/On--device_AI-412991?style=flat-square&logo=openai&logoColor=white" alt="On-device AI" />
</p>

컴퓨터 비전 · 카메라 및 영상 처리 · 온디바이스 분석 · 초분광 영상 복원
