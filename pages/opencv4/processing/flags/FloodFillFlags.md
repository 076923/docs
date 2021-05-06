---
title: 영역 채우기 플래그
sidebar: opencv4_sidebar
permalink: FloodFillFlags
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
| `FLOODFILL_FIXED_RANGE` | 영역 채우기 조건에 부합하는 영역만 채움 |
| `FLOODFILL_MASK_ONLY` | 입력 이미지를 변경하지 않고 마스크만 적용 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `FloodFillFlags.Link4` | 브레젠험 4 연결 방식 |
| `FloodFillFlags.Link8` |브레젠험 8 연결 방식 |
| `FloodFillFlags.FixedRange` | 영역 채우기 조건에 부합하는 영역만 채움 |
| `FloodFillFlags.MaskOnly` | 입력 이미지를 변경하지 않고 마스크만 적용 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.FLOODFILL_FIXED_RANGE` | 영역 채우기 조건에 부합하는 영역만 채움 |
| `cv2.FLOODFILL_MASK_ONLY` | 입력 이미지를 변경하지 않고 마스크만 적용 |

</div>
</div>

<br>

### 요약(Summary)

> 영역 채우기 방식을 설정합니다.
