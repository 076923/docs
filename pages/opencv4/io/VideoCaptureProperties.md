---
title: 비디오 속성 플래그
sidebar: opencv4_sidebar
permalink: VideoCaptureProperties
folder: opencv4
---

<ul id="profileTabs" class="nav nav-tabs">
    <li class="active"><a class="noCrossRef" href="#L1" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">C++</a></li>
    <li><a class="noCrossRef" href="#L2" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">C#</a></li>
    <li><a class="noCrossRef" href="#L3" data-toggle="tab" style="width: 100px; text-align: center; font-weight: 600; font-size: 15px;">Python</a></li>
</ul>

<div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="L1" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `CAP_PROP_POS_MSEC` | 비디오의 현재 위치(밀리초) 또는 타임스탬프 |
| `CAP_PROP_POS_FRAMES` | 비디오의 현재 프레임 |
| `CAP_PROP_POS_AVI_RATIO` | 비디오 내의 상대적 위치(0.0 ~ 1.0) |
| `CAP_PROP_FRAME_WIDTH` | 비디오 프레임 너비 |
| `CAP_PROP_FRAME_HEIGHT` | 비디오 프레임 높이 |
| `CAP_PROP_FPS` | 비디오 프레임 속도 |
| `CAP_PROP_FOURCC` | 비디오 코덱 |
| `CAP_PROP_FRAME_COUNT` | 비디오 총 프레임 수 |
| `CAP_PROP_FORMAT` | VideoCapture.retrieve로반환된 Mat 객체의 형식 |
| `CAP_PROP_MODE` | 현재 비디오의 백엔드 값 |
| `CAP_PROP_BRIGHTNESS` | 카메라의 밝기 설정 |
| `CAP_PROP_CONTRAST` | 카메라의 대비 설정 |
| `CAP_PROP_SATURATION` | 카메라의 채도 설정 |
| `CAP_PROP_HUE` | 카메라의 색상 설정 |
| `CAP_PROP_GAIN` | 카메라의 게인 설정 |
| `CAP_PROP_EXPOSURE` | 카메라의 노출 설정 |
| `CAP_PROP_CONVERT_RGB` | 비디오 프레임의 RGB 변환 유/무 |
| `CAP_PROP_WHITE_BALANCE_BLUE_U` | 화이트 밸런스 BlueU 설정(지원되지 않음) |
| `CAP_PROP_RECTIFICATION` | 스테레오 카메라 용 정류 플래그(DC1394 v2.x 백엔드만 지원) |
| `CAP_PROP_MONOCHROME` | 카메라의 단색화 설정 | 
| `CAP_PROP_SHARPNESS` | 카메라의 선명도 설정 | 
| `CAP_PROP_AUTO_EXPOSURE` | 카메라의 자동 노출 설정 |
| `CAP_PROP_GAMMA` | 카메라의 감마 설정 |
| `CAP_PROP_TEMPERATURE` | 열화상 카메라의 온도 설정 |
| `CAP_PROP_TRIGGER` | 카메라의 트리거 설정 | 
| `CAP_PROP_TRIGGER_DELAY` | 카메라의 트리거 지연 설정 |
| `CAP_PROP_WHITE_BALANCE_RED_V` | 화이트 밸런스 RedV 설정(지원되지 않음) | 
| `CAP_PROP_ZOOM` | 카메라의 줌 설정 |
| `CAP_PROP_FOCUS` | 카메라의 포커스 설정 |
| `CAP_PROP_GUID` | 카메라 장치 GUID 설정 |
| `CAP_PROP_ISO_SPEED` | 카메라 ISO 감도 설정 |
| `CAP_PROP_BACKLIGHT` | 카메라 백라이트 설정 | 
| `CAP_PROP_PAN` | 카메라 팬 설정 |
| `CAP_PROP_TILT` | 카메라 틸트 설정 |
| `CAP_PROP_ROLL` | 카메라 롤 설정 | 
| `CAP_PROP_IRIS` | 카메라 조리개 설정 |
| `CAP_PROP_SETTINGS` | 카메라 속성 설정 팝업 표시 유/무 |
| `CAP_PROP_BUFFERSIZE` | 카메라 버퍼 사이즈 설정 |
| `CAP_PROP_AUTOFOCUS` | 카메라 자동 포커스 설정 |
| `CAP_PROP_SAR_NUM` | 샘플 종횡비 Num 설정 |
| `CAP_PROP_SAR_DEN` | 샘플 종횡비 Den 설정 |
| `CAP_PROP_BACKEND` | 카메라 백엔드 설정 |
| `CAP_PROP_CHANNEL` | 비디오 채널 설정 |
| `CAP_PROP_AUTO_WB` | 자동 화이트 밸런스 설정 |
| `CAP_PROP_WB_TEMPERATURE` | 화이트 밸런스 색온도 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `VideoCaptureProperties.PosMsec` | 비디오의 현재 위치(밀리초) 또는 타임스탬프 |
| `VideoCaptureProperties.PosFrames` | 비디오의 현재 프레임 |
| `VideoCaptureProperties.PosAviRatio` | 비디오 내의 상대적 위치(0.0 ~ 1.0) |
| `VideoCaptureProperties.FrameWidth` | 비디오 프레임 너비 |
| `VideoCaptureProperties.FrameHeight` | 비디오 프레임 높이 |
| `VideoCaptureProperties.Fps` | 비디오 프레임 속도 |
| `VideoCaptureProperties.FourCC` | 비디오 코덱 |
| `VideoCaptureProperties.FrameCount` | 비디오 총 프레임 수 |
| `VideoCaptureProperties.Format` | VideoCapture.retrieve로 반환된 Mat 객체의 형식 |
| `VideoCaptureProperties.Mode` | 현재 비디오의 백엔드 값 |
| `VideoCaptureProperties.Brightness` | 카메라의 밝기 설정 |
| `VideoCaptureProperties.Contrast` | 카메라의 대비 설정 |
| `VideoCaptureProperties.Saturation` | 카메라의 채도 설정 |
| `VideoCaptureProperties.Hue` | 카메라의 색상 설정 |
| `VideoCaptureProperties.Gain` | 카메라의 게인 설정 |
| `VideoCaptureProperties.Exposure` | 카메라의 노출 설정 |
| `VideoCaptureProperties.ConvertRgb` | 비디오 프레임의 RGB 변환 유/무 |
| `VideoCaptureProperties.WhiteBalanceBlueU` | 화이트 밸런스 BlueU 설정(지원되지 않음) |
| `VideoCaptureProperties.Rectification` | 스테레오 카메라 용 정류 플래그(DC1394 v2.x 백엔드만 지원) |
| `VideoCaptureProperties.Monocrome` | 카메라의 단색화 설정 | 
| `VideoCaptureProperties.Sharpness` | 카메라의 선명도 설정 | 
| `VideoCaptureProperties.AutoExposure` | 카메라의 자동 노출 설정 |
| `VideoCaptureProperties.Gamma` | 카메라의 감마 설정 |
| `VideoCaptureProperties.Temperature` | 열화상 카메라의 온도 설정 |
| `VideoCaptureProperties.Trigger` | 카메라의 트리거 설정 | 
| `VideoCaptureProperties.TriggerDelay` | 카메라의 트리거 지연 설정 |
| `VideoCaptureProperties.WhiteBalanceRedV` | 화이트 밸런스 RedV 설정(지원되지 않음) | 
| `VideoCaptureProperties.Zoom` | 카메라의 줌 설정 |
| `VideoCaptureProperties.Focus` | 카메라의 포커스 설정 |
| `VideoCaptureProperties.Guid` | 카메라 장치 GUID 설정 |
| `VideoCaptureProperties.IsoSpeed` | 카메라 ISO 감도 설정 |
| `VideoCaptureProperties.BackLight` | 카메라 백라이트 설정 | 
| `VideoCaptureProperties.Pan` | 카메라 팬 설정 |
| `VideoCaptureProperties.Tilt` | 카메라 틸트 설정 |
| `VideoCaptureProperties.Roll` | 카메라 롤 설정 | 
| `VideoCaptureProperties.Iris` | 카메라 조리개 설정 |
| `VideoCaptureProperties.Settings` | 카메라 속성 설정 팝업 |
| `VideoCaptureProperties.BufferSize` | 카메라 버퍼 사이즈 설정 |
| `VideoCaptureProperties.AutoFocus` | 카메라 자동 포커스 설정 |
| `VideoCaptureProperties.SARNum` | 샘플 종횡비 Num 설정 |
| `VideoCaptureProperties.SARDen` | 샘플 종횡비 Den 설정 |
| `VideoCaptureProperties.Backend` | 카메라 백엔드 설정 |
| `VideoCaptureProperties.Channel` | 비디오 채널 설정 |
| `VideoCaptureProperties.AutoWB` | 자동 화이트 밸런스 설정 |
| `VideoCaptureProperties.WBTemperature` | 화이트 밸런스 색온도 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.CAP_PROP_POS_MSEC` | 비디오의 현재 위치(밀리초) 또는 타임스탬프 |
| `cv2.CAP_PROP_POS_FRAMES` | 비디오의 현재 프레임 |
| `cv2.CAP_PROP_POS_AVI_RATIO` | 비디오 내의 상대적 위치(0.0 ~ 1.0) |
| `cv2.CAP_PROP_FRAME_WIDTH` | 비디오 프레임 너비 |
| `cv2.CAP_PROP_FRAME_HEIGHT` | 비디오 프레임 높이 |
| `cv2.CAP_PROP_FPS`  | 비디오 프레임 속도 |
| `cv2.CAP_PROP_FOURCC` | 비디오 코덱 |
| `cv2.CAP_PROP_FRAME_COUNT` | 비디오 총 프레임 수 |
| `cv2.CAP_PROP_FORMAT` | VideoCapture.retrieve로 반환된 Mat 객체의 형식 |
| `cv2.CAP_PROP_MODE` | 현재 비디오의 백엔드 값 |
| `cv2.CAP_PROP_BRIGHTNESS` | 카메라의 밝기 설정 |
| `cv2.CAP_PROP_CONTRAST` | 카메라의 대비 설정 |
| `cv2.CAP_PROP_SATURATION` | 카메라의 채도 설정 |
| `cv2.CAP_PROP_HUE` | 카메라의 색상 설정 |
| `cv2.CAP_PROP_GAIN` | 카메라의 게인 설정 |
| `cv2.CAP_PROP_EXPOSURE` | 카메라의 노출 설정 |
| `cv2.CAP_PROP_CONVERT_RGB` | 비디오 프레임의 RGB 변환 유/무 |
| `cv2.CAP_PROP_WHITE_BALANCE_BLUE_U` | 화이트 밸런스 BlueU 설정(지원되지 않음) |
| `cv2.CAP_PROP_RECTIFICATION` | 스테레오 카메라 용 정류 플래그(DC1394 v2.x 백엔드만 지원) |
| `cv2.CAP_PROP_MONOCHROME` | 카메라의 단색화 설정 | 
| `cv2.CAP_PROP_SHARPNESS` | 카메라의 선명도 설정 | 
| `cv2.CAP_PROP_AUTO_EXPOSURE` | 카메라의 자동 노출 설정 |
| `cv2.CAP_PROP_GAMMA` | 카메라의 감마 설정 |
| `cv2.CAP_PROP_TEMPERATURE` | 열화상 카메라의 온도 설정 |
| `cv2.CAP_PROP_TRIGGER` | 카메라의 트리거 설정 | 
| `cv2.CAP_PROP_TRIGGER_DELAY` | 카메라의 트리거 지연 설정 |
| `cv2.CAP_PROP_WHITE_BALANCE_RED_V` | 화이트 밸런스 RedV 설정(지원되지 않음) | 
| `cv2.CAP_PROP_ZOOM` | 카메라의 줌 설정 |
| `cv2.CAP_PROP_FOCUS` | 카메라의 포커스 설정 |
| `cv2.CAP_PROP_GUID` | 카메라 장치 GUID 설정 |
| `cv2.CAP_PROP_ISO_SPEED` | 카메라 ISO 감도 설정 |
| `cv2.CAP_PROP_BACKLIGHT` | 카메라 백라이트 설정 | 
| `cv2.CAP_PROP_PAN` | 카메라 팬 설정 |
| `cv2.CAP_PROP_TILT` | 카메라 틸트 설정 |
| `cv2.CAP_PROP_ROLL` | 카메라 롤 설정 | 
| `cv2.CAP_PROP_IRIS` | 카메라 조리개 설정 |
| `cv2.CAP_PROP_SETTINGS` | 카메라 속성 설정 팝업 표시 유/무 |
| `cv2.CAP_PROP_BUFFERSIZE` | 카메라 버퍼 사이즈 설정 |
| `cv2.CAP_PROP_AUTOFOCUS` | 카메라 자동 포커스 설정 |
| `cv2.CAP_PROP_SAR_NUM` | 샘플 종횡비 Num 설정 |
| `cv2.CAP_PROP_SAR_DEN` | 샘플 종횡비 Den 설정 |
| `cv2.CAP_PROP_BACKEND` | 카메라 백엔드 설정 |
| `cv2.CAP_PROP_CHANNEL` | 비디오 채널 설정 |
| `cv2.CAP_PROP_AUTO_WB` | 자동 화이트 밸런스 설정 |
| `cv2.CAP_PROP_WB_TEMPERATURE` | 화이트 밸런스 색온도 |

</div>
</div>

### 요약(Summary)

> 비디오 API 백엔드를 설정합니다.