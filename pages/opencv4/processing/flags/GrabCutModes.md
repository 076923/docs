---
title: 그랩 컷 플래그
sidebar: opencv4_sidebar
permalink: GrabCutModes
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
| `GC_INIT_WITH_RECT` | 관심 영역을 활용해 모델과 마스크를 초기화 |
| `GC_INIT_WITH_MASK` | 입력된 마스크를 활용해 모델을 초기화 |
| `GC_EVAL` | 새로 계산된 모델을 사용하지 않음 |
| `GC_EVAL_FREEZE_MODEL` | 알고리즘을 고정 모델로 한 번만 실행 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `GrabCutModes.InitWithRect` | 관심 영역을 활용해 모델과 마스크를 초기화 |
| `GrabCutModes.InitWithMask` | 입력된 마스크를 활용해 모델을 초기화 |
| `GrabCutModes.Eval` | 새로 계산된 모델을 사용하지 않음 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.GC_INIT_WITH_RECT` | 관심 영역을 활용해 모델과 마스크를 초기화 |
| `cv2.GC_INIT_WITH_MASK` | 입력된 마스크를 활용해 모델을 초기화 |
| `cv2.GC_EVAL` | 새로 계산된 모델을 사용하지 않음 |
| `cv2.GC_EVAL_FREEZE_MODEL` | 알고리즘을 고정 모델로 한 번만 실행 |

</div>
</div>

<br>

### 요약(Summary)

> 그랩 컷 방식을 설정합니다.
