# 바이페달 휠 로봇 — 하드웨어

자기 균형 바이페달 휠 로봇의 오픈소스 하드웨어 프로젝트입니다.
[CERN Open Hardware Licence v2](LICENSE) 라이선스로 공개합니다.

---

## 저장소 구조

```
/
├── CAD/
│   ├── Assembly/          # 전체 조립 및 서브 어셈블리 CAD 파일
│   ├── battery_and_cage/  # 배터리 홀더 및 케이지 CAD 파일
│   └── Print/             # 3D 출력 파트 (FDM, PLA, 블랙)
├── BOM/
│   └── BOM.md             # 부품 목록
├── README.md
└── README_ko.md
```

> **CAD 파일은 [GitHub Releases](../../releases)를 통해 배포됩니다.**
> 레포지토리 내 CAD 폴더는 구조 정의용입니다.
> 최신 릴리즈를 다운로드하면 F3D, STEP, STL, 3MF 파일을 모두 받을 수 있습니다.

---

## 3D 프린트 파트

모든 출력 파트는 블랙 PLA FDM 출력을 기준으로 설계되었습니다.
로봇은 **좌우 대칭 구조**로, 같은 파일을 양쪽 다리에 동일하게 사용합니다.

| 파일 | 다리당 수량 | 비고 |
|------|-----------|------|
| BalanceArm_R | 2 | |
| Head_R | 1 | |
| LowerArm_Bearing_R | 1 | |
| LowerArm_Motor_R | 1 | |
| UpperArm_Bearing_R | 1 | |
| UpperArm_Motor_R | 1 | |
| Wheel_R | 1 | |

---

## 어셈블리 파일

| 파일 | 설명 |
|------|------|
| assembled_with_removable_components | 전체 조립 |
| head_cover | 헤드 커버 패널 |
| Wheel Robot_origin set | 헤드 커버 및 배터리 미포함 기초 골격 |

CAD 파일은 F3D, STEP, STL, 3MF 포맷으로 제공됩니다.

---

## 패널

배선판과 헤드 커버는 **포맥스(PVC 폼보드) 3t, 300×450mm**를 재단하여 사용합니다.
- 헤드 커버는 135° 브래킷으로 프레임에 연결합니다.
- 3D 프린터가 있다면 출력해서 대체할 수도 있습니다.
- 다층 배선판은 **45mm PCB 지지볼트**를 기둥처럼 사용해 레이어 간 연결합니다.

---

## 주요 부품

전체 부품 목록은 [BOM/BOM.md](BOM/BOM.md)를 참고하세요.

### 필수
- **모터**: Robstride O4 ×4

### 선택 (사용자 필요에 따라)
- **라이다**: Unitree L2
- **카메라**: 일반 모듈 또는 Intel RealSense D435

---

## 라이선스

CERN Open Hardware Licence Version 2 — [LICENSE](LICENSE) 참고.
