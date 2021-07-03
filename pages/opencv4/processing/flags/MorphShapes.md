---
title: 구조 요소 플래그
sidebar: opencv4_sidebar
permalink: MorphShapes
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
| `MORPH_RECT` | 직사각형 형태로 모든 $$ i,\ j $$의 요소에 대해 $$ K_{i, j} = 1 $$ |
| `MORPH_CROSS` | 십자가 형태로 고정점의 $$ i,\ j $$를 기준으로 $$ K_{i, j} = 1 $$ |
| `MORPH_ELLIPSE` | 타원 형태로 커널의 너비와 높이를 축으로 하는 타원에 대해 $$ K_{i, j} = 1 $$ |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `MorphShapes.Rect` | 직사각형 형태로 모든 $$ i,\ j $$의 요소에 대해 $$ K_{i, j} = 1 $$ |
| `MorphShapes.Cross` | 십자가 형태로 고정점의 $$ i,\ j $$를 기준으로 $$ K_{i, j} = 1 $$ |
| `MorphShapes.Ellipse` | 타원 형태로 커널의 너비와 높이를 축으로 하는 타원에 대해 $$ K_{i, j} = 1 $$ |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.MORPH_RECT` | 직사각형 형태로 모든 $$ i,\ j $$의 요소에 대해 $$ K_{i, j} = 1 $$ |
| `cv2.MORPH_CROSS` | 십자가 형태로 고정점의 $$ i,\ j $$를 기준으로 $$ K_{i, j} = 1 $$ |
| `cv2.MORPH_ELLIPSE` | 타원 형태로 커널의 너비와 높이를 축으로 하는 타원에 대해 $$ K_{i, j} = 1 $$ |

</div>
</div>

<br>

### 요약(Summary)

> 구조 요소 형태를 설정합니다.
