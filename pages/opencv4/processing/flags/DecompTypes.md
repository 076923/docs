---
title: 행렬 분해 플래그
sidebar: opencv4_sidebar
permalink: DecompTypes
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
| `DECOMP_LU` | LU 분해(가우스 소거) |
| `DECOMP_SVD` | 특잇값 분해 |
| `DECOMP_EIG` | 고윳값 분해 |
| `DECOMP_CHOLESKY` | 숄레스키 분해 |
| `DECOMP_QR` | QR 인수 분해 |
| `DECOMP_NORMAL` | 노멀 분해(src1ㆍdst = src2 방정식 사용) |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `DecompTypes.LU` | LU 분해(가우스 소거) |
| `DecompTypes.SVD` | 특잇값 분해 |
| `DecompTypes.Eig` | 고윳값 분해 |
| `DecompTypes.Cholesky` | 숄레스키 분해 |
| `DecompTypes.QR` | QR 인수 분해 |
| `DecompTypes.Normal` | 노멀 분해(src1ㆍdst = src2 방정식 사용) |


</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.DECOMP_LU` | LU 분해(가우스 소거) |
| `cv2.DECOMP_SVD` | 특잇값 분해 |
| `cv2.DECOMP_EIG` | 고윳값 분해 |
| `cv2.DECOMP_CHOLESKY` | 숄레스키 분해 |
| `cv2.DECOMP_QR` | QR 인수 분해 |
| `cv2.DECOMP_NORMAL` | 노멀 분해(src1ㆍdst = src2 방정식 사용) |

</div>
</div>

<br>

### 요약(Summary)

> 행렬 분해 방식을 설정합니다.
