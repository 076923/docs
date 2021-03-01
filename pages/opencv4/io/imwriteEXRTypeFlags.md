---
title: EXR 형식 플래그
sidebar: opencv4_sidebar
permalink: imwriteEXRTypeFlags
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
| `IMWRITE_EXR_TYPE_HALF` | FP16으로 저장 |
| `IMWRITE_EXR_TYPE_FLOAT` | FP32로 저장 |


</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `ImwriteEXRTypeFlags.TypeHalf` | FP16으로 저장 |
| `ImwriteEXRTypeFlags.TypeFloat` | FP32로 저장 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.IMWRITE_EXR_TYPE_HALF` | FP16으로 저장 |
| `cv2.IMWRITE_EXR_TYPE_FLOAT` | FP32로 저장 |

</div>
</div>

### 요약(Summary)

> EXR 저장 방식을 설정합니다.