---
title: 거리 변환 라벨링 방식 플래그
sidebar: opencv4_sidebar
permalink: DistanceTransformLabelTypes
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
| `DIST_LABEL_CCOMP` | 연결된 구성 요소에 가장 가까운 0이 아닌 모든 픽셀은 동일한 레이블을 할당 |
| `DIST_LABEL_PIXEL` | 가장 가까운 0이 아닌 모든 픽셀은 자체 레이블을 할당 |


</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `DistanceTransformLabelTypes.CComp` | 연결된 구성 요소에 가장 가까운 0이 아닌 모든 픽셀은 동일한 레이블을 할당 |
| `DistanceTransformLabelTypes.Pixel` | 가장 가까운 0이 아닌 모든 픽셀은 자체 레이블을 할당 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.DIST_LABEL_CCOMP` | 연결된 구성 요소에 가장 가까운 0이 아닌 모든 픽셀은 동일한 레이블을 할당 |
| `cv2.DIST_LABEL_PIXEL` | 가장 가까운 0이 아닌 모든 픽셀은 자체 레이블을 할당 |


</div>
</div>

<br>

### 요약(Summary)

> 거리 변환 라벨링 방식을 설정합니다.
