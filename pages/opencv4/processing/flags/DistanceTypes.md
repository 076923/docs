---
title: 거리 계산 방식 플래그
sidebar: opencv4_sidebar
permalink: DistanceTypes
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
| `DIST_USER` | 사용자 정의 거리 계산 방식 |
| `DIST_L1` | $$ distance = \| x_1 - x_2 \| + \| y_1 - y_2 \| $$ |
| `DIST_L2` | $$ distance = \sqrt{\sum_{i=1}^n (x_i - y_i)^2} $$ |
| `DIST_C` | $$ distance = max(\| x1 - x2 \|, \| y1 - y2 \|) $$ |
| `DIST_L12` | $$ distance =  2\sqrt{1+\frac{x^2}{2}} - 2 $$ |
| `DIST_FAIR` |  $$ distance = c^2(\frac{\|x\|}{c}-\log(1+\frac{\|x\|}{c})),\ ​c = 1.3998 $$ |
| `DIST_WELSCH` | $$ distance = \frac{c^2}{2}(1-\exp(-(\frac{x}{c})^2)),\ c = 2.9846 $$ |
| `DIST_HUBER` | $$ distance = \|x\|<c \ ? \ \frac{x^2}{2} \ : \ c(\|x\|-\frac{c}{2}),\ c = 1.345 $$ |


</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `DistanceTypes.User` | 사용자 정의 거리 계산 방식 |
| `DistanceTypes.L1` | $$ distance = \| x_1 - x_2 \| + \| y_1 - y_2 \| $$ |
| `DistanceTypes.L2` | $$ distance = \sqrt{\sum_{i=1}^n (x_i - y_i)^2} $$ |
| `DistanceTypes.C` | $$ distance = max(\| x1 - x2 \|, \| y1 - y2 \|) $$ |
| `DistanceTypes.L12` | $$ distance =  2\sqrt{1+\frac{x^2}{2}} - 2 $$ |
| `DistanceTypes.Fair` |  $$ distance = c^2(\frac{\|x\|}{c}-\log(1+\frac{\|x\|}{c})),\ ​c = 1.3998 $$ |
| `DistanceTypes.Welsch` | $$ distance = \frac{c^2}{2}(1-\exp(-(\frac{x}{c})^2)),\ c = 2.9846 $$ |
| `DistanceTypes.Huber` | $$ distance = \|x\|<c \ ? \ \frac{x^2}{2} \ : \ c(\|x\|-\frac{c}{2}),\ c = 1.345 $$ |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.DIST_USER` | 사용자 정의 거리 계산 방식 |
| `cv2.DIST_L1` | $$ distance = \| x_1 - x_2 \| + \| y_1 - y_2 \| $$ |
| `cv2.DIST_L2` | $$ distance = \sqrt{\sum_{i=1}^n (x_i - y_i)^2} $$ |
| `cv2.DIST_C` | $$ distance = max(\| x1 - x2 \|, \| y1 - y2 \|) $$ |
| `cv2.DIST_L12` | $$ distance =  2\sqrt{1+\frac{x^2}{2}} - 2 $$ |
| `cv2.DIST_FAIR` |  $$ distance = c^2(\frac{\|x\|}{c}-\log(1+\frac{\|x\|}{c})),\ ​c = 1.3998 $$ |
| `cv2.DIST_WELSCH` | $$ distance = \frac{c^2}{2}(1-\exp(-(\frac{x}{c})^2)),\ c = 2.9846 $$ |
| `cv2.DIST_HUBER` | $$ distance = \|x\|<c \ ? \ \frac{x^2}{2} \ : \ c(\|x\|-\frac{c}{2}),\ c = 1.345 $$ |

</div>
</div>

<br>

### 요약(Summary)

> 거리 계산 방식을 설정합니다.
