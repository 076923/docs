---
title: 이미지 읽기 모드
sidebar: opencv4_sidebar
permalink: imreadModes
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
| `IMREAD_UNCHANGED` | 알파 채널을 포함해서 이미지 반환(알파 채널이 없을 경우 3채널로 반환) | 
| `IMREAD_GRAYSCALE` | 내부 코덱을 사용하여 단일 채널 그레이스케일 이미지로 반환 | 
| `IMREAD_COLOR` | 다중 채널 색상 이미지로 반환 | 
| `IMREAD_ANYDEPTH` | 정밀도가 있다면 16 비트 또는 32 비트 이미지로 반환(없다면 8 비트 이미지로 반환) | 
| `IMREAD_ANYCOLOR` | 채널이 있다면 해당 채널 수로 반환(없다면 3채널 이미지로 반환) | 
| `IMREAD_LOAD_GDAL` | GDAL 드라이버를 사용하여 반환 | 
| `IMREAD_REDUCED_GRAYSCALE_2` | 크기를 1/2로 줄인 후 그레이스케일 적용 | 
| `IMREAD_REDUCED_GRAYSCALE_4` | 크기를 1/4로 줄인 후 그레이스케일 적용 | 
| `IMREAD_REDUCED_GRAYSCALE_8` | 크기를 1/8로 줄인 후 그레이스케일 적용 | 
| `IMREAD_REDUCED_COLOR_2` | 크기를 1/2로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `IMREAD_REDUCED_COLOR_4` | 크기를 1/4로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `IMREAD_REDUCED_COLOR_8` | 크기를 1/8로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `IMREAD_IGNORE_ORIENTATION` | EXIF의 방향 플래그에 따라 이미지를 회전하지 않음 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `ImreadModes.Unchanged` | 알파 채널을 포함해서 이미지 반환(알파 채널이 없을 경우 3채널로 반환) | 
| `ImreadModes.Grayscale` | 내부 코덱을 사용하여 단일 채널 그레이스케일 이미지로 반환 | 
| `ImreadModes.Color` | 다중 채널 색상 이미지로 반환 | 
| `ImreadModes.AnyDepth` | 정밀도가 있다면 16 비트 또는 32 비트 이미지로 반환(없다면 8 비트 이미지로 반환) | 
| `ImreadModes.AnyColor` | 채널이 있다면 해당 채널 수로 반환(없다면 3채널 이미지로 반환) | 
| `ImreadModes.LoadGdal` | GDAL 드라이버를 사용하여 반환 | 
| `ImreadModes.ReducedGrayscale2` | 크기를 1/2로 줄인 후 그레이스케일 적용 | 
| `ImreadModes.ReducedGrayscale4` | 크기를 1/4로 줄인 후 그레이스케일 적용 | 
| `ImreadModes.ReducedGrayscale8` | 크기를 1/8로 줄인 후 그레이스케일 적용 | 
| `ImreadModes.ReducedColor2` | 크기를 1/2로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `ImreadModes.ReducedColor4` | 크기를 1/4로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `ImreadModes.ReducedColor8` | 크기를 1/8로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `ImreadModes.IgnoreOrientation` | EXIF의 방향 플래그에 따라 이미지를 회전하지 않음 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.IMREAD_UNCHANGED` | 알파 채널을 포함해서 이미지 반환(알파 채널이 없을 경우 3채널로 반환) | 
| `cv2.IMREAD_GRAYSCALE` | 내부 코덱을 사용하여 단일 채널 그레이스케일 이미지로 반환 | 
| `cv2.IMREAD_COLOR` | 다중 채널 색상 이미지로 반환 | 
| `cv2.IMREAD_ANYDEPTH` | 정밀도가 있다면 16 비트 또는 32 비트 이미지로 반환(없다면 8 비트 이미지로 반환) | 
| `cv2.IMREAD_ANYCOLOR` | 채널이 있다면 해당 채널 수로 반환(없다면 3채널 이미지로 반환) | 
| `cv2.IMREAD_LOAD_GDAL` | GDAL 드라이버를 사용하여 반환 | 
| `cv2.IMREAD_REDUCED_GRAYSCALE_2` | 크기를 1/2로 줄인 후 그레이스케일 적용 | 
| `cv2.IMREAD_REDUCED_GRAYSCALE_4` | 크기를 1/4로 줄인 후 그레이스케일 적용 | 
| `cv2.IMREAD_REDUCED_GRAYSCALE_8` | 크기를 1/8로 줄인 후 그레이스케일 적용 | 
| `cv2.IMREAD_REDUCED_COLOR_2` | 크기를 1/2로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `cv2.IMREAD_REDUCED_COLOR_4` | 크기를 1/4로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `cv2.IMREAD_REDUCED_COLOR_8` | 크기를 1/8로 줄인 후 다중 채널 색상 이미지로 반환 | 
| `cv2.IMREAD_IGNORE_ORIENTATION` | EXIF의 방향 플래그에 따라 이미지를 회전하지 않음 |

</div>
</div>

### 요약(Summary)

> 이미지 변환 방식을 설정합니다.