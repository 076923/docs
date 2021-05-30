---
title: 내삽 플래그
sidebar: opencv4_sidebar
permalink: InterpolationFlags
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
| `INTER_NEAREST` | 최근접 이웃 보간법 |
| `INTER_LINEAR` | 이중 선형 보간법 |
| `INTER_CUBIC` | 4×4 바이 큐빅 보간법 |
| `INTER_AREA` | 영역 보간법 |
| `INTER_LANCZOS4` | 8×8 란초스 보간법 |
| `INTER_NEAREST_EXACT` | 비트 단위 최근접 이웃 선형 보간법 |
| `INTER_LINEAR_EXACT` | 비트 단위 이중 선형 보간법 |
| `INTER_MAX` | 마스크 플래그 |
| `WARP_FILL_OUTLIERS` | 이상치에 해당하는 경우 0으로 설정 |
| `WARP_INVERSE_MAP` | 역변환 플래그 |


</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `InterpolationFlags.Nearest` | 최근접 이웃 보간법 |
| `InterpolationFlags.Linear` | 이중 선형 보간법 |
| `InterpolationFlags.Cubic` | 4×4 바이 큐빅 보간법 |
| `InterpolationFlags.Area` | 영역 보간법 |
| `InterpolationFlags.Lanczos4` | 8×8 란초스 보간법 |
| `InterpolationFlags.LinearNearest` | <a data-toggle="tooltip" data-original-title="{{site.data.glossary.Not_supported}}">비트 단위 최근접 이웃 선형 보간법</a> |
| `InterpolationFlags.LinearExact` | 비트 단위 이중 선형 보간법 |
| `InterpolationFlags.Max` | 마스크 플래그 |
| `InterpolationFlags.WarpFillOutliers` | 이상치에 해당하는 경우 0으로 설정 |
| `InterpolationFlags.WarpInverseMap` | 역변환 플래그 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.INTER_NEAREST` | 최근접 이웃 보간법 |
| `cv2.INTER_LINEAR` | 이중 선형 보간법 |
| `cv2.INTER_CUBIC` | 4×4 바이 큐빅 보간법 |
| `cv2.INTER_AREA` | 영역 보간법 |
| `cv2.INTER_LANCZOS4` | 8×8 란초스 보간법 |
| `cv2.INTER_NEAREST_EXACT` | 비트 단위 최근접 이웃 선형 보간법 |
| `cv2.INTER_LINEAR_EXACT` | 비트 단위 이중 선형 보간법 |
| `cv2.INTER_MAX` | 마스크 플래그 |
| `cv2.WARP_FILL_OUTLIERS` | 이상치에 해당하는 경우 0으로 설정 |
| `cv2.WARP_INVERSE_MAP` | 역변환 플래그 |

</div>
</div>

<br>

### 요약(Summary)

> 내삽(보간) 방식을 설정합니다.
