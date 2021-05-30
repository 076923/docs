---
title: 외삽 플래그
sidebar: opencv4_sidebar
permalink: BorderTypes
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
| `BORDER_CONSTANT` | 고정값으로 픽셀을 확장<br>`iiiiii | abcdefgh | iiiiii` |
| `BORDER_REPLICATE` | 테두리 픽셀을 복사해서 확장<br>`aaaaaa | abcdefgh | hhhhhh` |
| `BORDER_REFLECT` | 픽셀을 반사해서 확장<br>`fedcba | abcdefgh | hgfedc` |
| `BORDER_WRAP` | 반대쪽 픽셀을 복사해서 확장<br>`cdefgh | abcdefgh | abcdef` |
| `BORDER_REFLECT_101` | 이중 픽셀을 만들지 않고 반사해서 확장<br>`gfedcb | abcdefgh | gfedcb` |
| `BORDER_DEFAULT` | Reflect101 방식을 사용<br>`gfedcb | abcdefgh | gfedcb` |
| `BORDER_TRANSPARENT` | 픽셀을 투명하게 해서 확장<br>`uvwxyz | abcdefgh | ijklmn` |
| `BORDER_ISOLATED` | 관심 영역(ROI) 밖은 고려하지 않음 |


</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `BorderTypes.Constant` | 고정값으로 픽셀을 확장<br>`iiiiii | abcdefgh | iiiiii` |
| `BorderTypes.Replicate` | 테두리 픽셀을 복사해서 확장<br>`aaaaaa | abcdefgh | hhhhhh` |
| `BorderTypes.Reflect` | 픽셀을 반사해서 확장<br>`fedcba | abcdefgh | hgfedc` |
| `BorderTypes.Wrap` | 반대쪽 픽셀을 복사해서 확장<br>`cdefgh | abcdefgh | abcdef` |
| `BorderTypes.Reflect101` | 이중 픽셀을 만들지 않고 반사해서 확장<br>`gfedcb | abcdefgh | gfedcb` |
| `BorderTypes.Default` | Reflect101 방식을 사용<br>`gfedcb | abcdefgh | gfedcb` |
| `BorderTypes.Transparent` | 픽셀을 투명하게 해서 확장<br>`uvwxyz | abcdefgh | ijklmn` |
| `BorderTypes.Isolated` | 관심 영역(ROI) 밖은 고려하지 않음 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.BORDER_CONSTANT` | 고정값으로 픽셀을 확장<br>`iiiiii | abcdefgh | iiiiii` |
| `cv2.BORDER_REPLICATE` | 테두리 픽셀을 복사해서 확장<br>`aaaaaa | abcdefgh | hhhhhh` |
| `cv2.BORDER_REFLECT` | 픽셀을 반사해서 확장<br>`fedcba | abcdefgh | hgfedc` |
| `cv2.BORDER_WRAP` | 반대쪽 픽셀을 복사해서 확장<br>`cdefgh | abcdefgh | abcdef` |
| `cv2.BORDER_REFLECT_101` | 이중 픽셀을 만들지 않고 반사해서 확장<br>`gfedcb | abcdefgh | gfedcb` |
| `cv2.BORDER_DEFAULT` | Reflect101 방식을 사용<br>`gfedcb | abcdefgh | gfedcb` |
| `cv2.BORDER_TRANSPARENT` | 픽셀을 투명하게 해서 확장<br>`uvwxyz | abcdefgh | ijklmn` |
| `cv2.BORDER_ISOLATED` | 관심 영역(ROI) 밖은 고려하지 않음 |

</div>
</div>

<br>

### 요약(Summary)

> 외삽(보외) 방식을 설정합니다.
