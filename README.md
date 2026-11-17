### 소프트웨어 개발자

# 이병현

**문제를 발견하고, 해결을 구현합니다.**

앱을 개발·출시하고, 컴퓨터비전과 딥러닝을 연구합니다.<br>
동국대학교 멀티미디어공학과 졸업 예정 개발자입니다.

**[포트폴리오](https://biyonghiyon.github.io/portfolio/)** · [이메일](mailto:pilot803@naver.com)

<br>

## 관심 분야와 역량

| 분야 | 내용 |
|---|---|
| **앱 · 웹 개발** | 기획부터 구현, 출시, 유지보수까지 경험했고 iOS·Android 앱과 실시간 웹 서비스를 직접 배포했습니다. |
| **컴퓨터비전** | 오픈소스 온디바이스 자세 추정(pose) 모델 여러 개를 직접 벤치마크해 비교하고, 모바일 기기에서 실시간으로 동작하는 영상 분석을 앱에 적용했습니다. |
| **딥러닝** | 영상 기반 오픈소스 팬샤프닝 모델을 재현하고, 위성영상을 대상으로 구조와 학습 방식을 바꿔 가며 성능을 개선하는 연구를 진행하고 있습니다. |
| **알고리즘** | 복잡한 문제를 작은 단위로 나누고, 더 효율적인 방법을 비교해 가며 풀어 갑니다. 프로그래밍기초와실습 과목에서 실습조교로 학생들의 실습을 도왔습니다. |

<br>

## 프로젝트

<img src="https://github.com/user-attachments/assets/f3f75e67-414c-4a6a-92f2-52b47f9badbd" alt="TopOut 아이콘" width="64" align="left">

### TopOut
모바일 앱 · iOS / Android 출시 · 2026.06 — 현재 · 개인 프로젝트

<br clear="left">

등반 시작부터 완등 순간까지 자동으로 찾아주는 실내 클라이밍 촬영 앱입니다. 긴 영상을 다시 돌려보며 장면을 찾는 대신, 기기 안에서 움직임과 자세를 분석해 필요한 구간만 골라 줍니다.

- App Store · Google Play 출시 (v3.0), 사용자 피드백으로 계속 업데이트
- 기기 내 자세 추정과 MobileSAM으로 매트 경계 자동 탐지
- 한 번의 촬영에서 여러 등반 시도를 자동으로 구분
- 영상을 서버로 보내지 않는 온디바이스 분석
- 9개 언어 지원, 한국 외 15개국에서 설치 (전체의 약 23%)

| 누적 설치 (광고 없음) | 최대 MAU (2026.09) | 월간 사용자 중 매주 사용 |
|:---:|:---:|:---:|
| **약 210회** | **약 110명** | **약 40%** |

<sub>클라이밍을 하는 사람만을 위한 앱이라 사용자 층이 좁고, 클라이머 대부분이 한 달에 2~3회 정도 클라이밍장에 가기 때문에 매일 쓰이는 앱이 아닙니다. 그래서 매일 사용(DAU) 대신 주간 재사용을 지표로 봤습니다. 월간 사용자 1명이 한 달에 약 2주 꼴로 앱을 열어, 운동하러 간 날 상당수를 TopOut으로 촬영합니다. 주간 사용 비율은 iOS 기준(사용 데이터 공유에 동의한 기기)입니다.</sub>

`Swift` · `Kotlin` · `Jetpack Compose` · `Apple Vision` · `MoveNet` · `MobileSAM`

**[소개 페이지](https://topout-portfolio.vercel.app/)** · [GitHub](https://github.com/BIYONGHIYON/TopOut-app) · [App Store](https://apps.apple.com/app/id6790163178) · [Google Play](https://play.google.com/store/apps/details?id=com.topout.cam)

<br>

### CtrS
딥러닝 연구 · 위성영상 팬샤프닝 · 2026.09 — 현재 · 팀장 · 4인

고해상도 흑백 위성영상(PAN)과 저해상도 다중분광영상(MS)을 합쳐 고해상도 컬러 영상을 복원하는 팬샤프닝 연구입니다. 동국대 종합설계1 프로젝트로 SSA-MRN의 성능을 개선하고 있습니다.

- 병렬 가지 · 축척 혼합 학습 · 관측 일치 사영으로 기준 모델 C2MS-SP 채택
- 원본 SSA-MRN 대비 RR PSNR QB +0.94 · GF2 +2.24 · WV3 +1.14 dB (3시드 평균)
- 학습하지 않은 센서(WV2)에서 +2.95 dB, 색 치우침 7.2% → 0.1% (밴드별 센서 보정)
- 연산을 66%로 줄인 경량판 C2MS-SP-Lite (C2MS-SP와 0.01–0.03 dB 차이)

<img src="https://raw.githubusercontent.com/BIYONGHIYON/CtrS/main/SSA-MRN/docs/images/c2ms_sp/WV2/full_scene_00.png" alt="WV2 장면 0 원본 크기 비교: LR MS·PAN 입력·원본 SSA-MRN·C2MS-SP·C2MS-SP-Lite·정답과 세 모델의 오차 지도" width="100%">

<sub>WV3로 학습한 모델을 학습하지 않은 센서 WV2에 적용한 RR 장면 0(seed 42)입니다. 위 줄은 입력과 각 모델의 결과·정답, 아래 줄은 오차 지도입니다(밝을수록 오차가 큼). 장면 PSNR은 원본 27.80 → C2MS-SP 30.90 dB입니다(밴드별 센서 보정 포함).</sub>

`PyTorch` · `Computer Vision` · `Pansharpening` · `Remote Sensing`

**[소개 페이지](https://biyonghiyon.github.io/CtrS/)** · [GitHub](https://github.com/BIYONGHIYON/CtrS) · [결과 비교 뷰어](https://biyonghiyon.github.io/CtrS-viewer/)

<br>

### NODE
게임 · 2.5D 로컬 협동 플랫포머 · 2026.04 — 2026.06 · 개인 프로젝트

두 우주비행사가 로프로 서로를 이어 우주를 탐험하는 2인 로컬 협동 게임입니다. 파트너나 지형에 로프를 걸고 스윙하며 퍼즐을 풀고, 흩어진 연료통을 모아 다음 행성으로 넘어갑니다.

- 파트너·지형에 거는 로프 스윙 액션
- 고중력 목성, 무중력 토성 등 행성마다 다른 중력
- 밀고 당기는 운석과 지형을 활용한 협동 퍼즐
- Windows · macOS 설치 파일 배포

https://github.com/user-attachments/assets/5ab698a2-caba-4773-ac90-e37cc6a2ec21

`Unity` · `C#` · `Local Co-op`

**[소개 페이지](https://biyonghiyon.github.io/NODE/)** · [GitHub](https://github.com/BIYONGHIYON/NODE) · [다운로드](https://github.com/BIYONGHIYON/NODE/releases/latest)

<br>

### Linkcast
웹 서비스 · 실시간 P2P 화면 공유 · 2026.09 — 2026.10 · 개인 프로젝트

USB 캡처보드나 화면 공유로 입력한 콘솔·PC 화면을 링크 하나로 공유하는 소규모 실시간 방송 서비스입니다. 송출자가 최대 5명에게 영상을 보내고, 모두가 브라우저에서 음성으로 대화할 수 있습니다.

- WebRTC P2P로 최대 1080p 60fps 초저지연 송출
- 송출자·참가자 전원이 참여하는 음성 통화
- 클릭·터치 드래그로 포인터를 공유하는 레이저 모드
- Cloudflare Workers · Durable Objects 기반 시그널링

<img src="https://raw.githubusercontent.com/BIYONGHIYON/portfolio/main/assets/linkcast-landing.jpg" alt="Linkcast 첫 화면: 캡처보드 연결 안내와 입력 설정, 링크 만들고 복사 버튼" width="100%">

<sub>Linkcast에 접속하면 처음 보이는 송출 화면입니다. 캡처보드를 연결하고 링크를 만들어 공유합니다.</sub>

`TypeScript` · `React` · `WebRTC` · `Cloudflare Workers` · `Durable Objects`

**[소개 페이지](https://biyonghiyon.github.io/linkcast/)** · [GitHub](https://github.com/BIYONGHIYON/linkcast) · [서비스 열기](https://linkcast.byeonghyeon383.workers.dev/)

<br>

## Contact

포트폴리오 [biyonghiyon.github.io/portfolio](https://biyonghiyon.github.io/portfolio/) · 이메일 [pilot803@naver.com](mailto:pilot803@naver.com)
