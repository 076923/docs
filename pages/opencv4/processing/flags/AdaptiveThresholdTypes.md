---
title: 적응형 이진화 플래그
sidebar: opencv4_sidebar
permalink: AdaptiveThresholdTypes
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
| `ADAPTIVE_THRESH_MEAN_C` | 블록 크기 영역의 모든 픽셀에 평균 가중치를 적용 |
| `ADAPTIVE_THRESH_MEAN_C` | 블록 크기 영역의 모든 픽셀에 중심점으로부터 거리에 대한 가우시안 가중치를 적용 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `AdaptiveThresholdTypes.MeanC` | 블록 크기 영역의 모든 픽셀에 평균 가중치를 적용 |
| `AdaptiveThresholdTypes.GaussianC` | 블록 크기 영역의 모든 픽셀에 중심점으로부터 거리에 대한 가우시안 가중치를 적용 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.ADAPTIVE_THRESH_MEAN_C` | 블록 크기 영역의 모든 픽셀에 평균 가중치를 적용 |
| `cv2.ADAPTIVE_THRESH_MEAN_C` | 블록 크기 영역의 모든 픽셀에 중심점으로부터 거리에 대한 가우시안 가중치를 적용 |

</div>
</div>

<br>

### 요약(Summary)

> 적응형 이진화 계산 방식을 설정합니다.
