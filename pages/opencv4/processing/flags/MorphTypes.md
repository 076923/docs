---
title: 모폴로지 연산 플래그
sidebar: opencv4_sidebar
permalink: MorphTypes
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
| `MORPH_DILATE` | 팽창 연산 |
| `MORPH_ERODE` | 침식 연산 |
| `MORPH_OPEN` | 열림 연산<br>$$ \text{dst} = \text{open}(\text{src}, \text{element}) = \text{dilate}(\text{erode}(\text{src}, \text{element})) $$ |
| `MORPH_CLOSE` | 닫힘 연산<br>$$ \text{dst} = \text{close}(\text{src}, \text{element}) = \text{erode}(\text{dilate}(\text{src}, \text{element})) $$ |
| `MORPH_GRADIENT` | 그라디언트 연산<br>$$ \text{dst} = \text{gradient}(\text{src}, \text{element}) = \text{dilate}(\text{src}, \text{element}) - \text{erode}(\text{src}, \text{element}) $$  |
| `MORPH_TOPHAT` | 탑 햇 연산<br>$$ \text{dst} = \text{tophat}(\text{src}, \text{element}) = \text{src} - \text{open}(\text{src}, \text{element}) $$ |
| `MORPH_BLACKHAT` | 블랙 햇 연산<br>$$ \text{dst} = \text{blackhat}(\text{src}, \text{element}) = \text{close}(\text{src}, \text{element}) - \text{src} $$ |
| `MORPH_HITMISS` | 히트미스 연산<br> `CV_8UC1` 형식의 이진 이미지만 가능 |

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `MorphTypes.Dilate` | 팽창 연산 |
| `MorphTypes.Erode` | 침식 연산 |
| `MorphTypes.Open` | 열림 연산<br>$$ \text{dst} = \text{open}(\text{src}, \text{element}) = \text{dilate}(\text{erode}(\text{src}, \text{element})) $$ |
| `MorphTypes.Close` | 닫힘 연산<br>$$ \text{dst} = \text{close}(\text{src}, \text{element}) = \text{erode}(\text{dilate}(\text{src}, \text{element})) $$ |
| `MorphTypes.Gradient` | 그라디언트 연산<br>$$ \text{dst} = \text{gradient}(\text{src}, \text{element}) = \text{dilate}(\text{src}, \text{element}) - \text{erode}(\text{src}, \text{element}) $$  |
| `MorphTypes.TopHat` | 탑 햇 연산<br>$$ \text{dst} = \text{tophat}(\text{src}, \text{element}) = \text{src} - \text{open}(\text{src}, \text{element}) $$ |
| `MorphTypes.BlackHat` | 블랙 햇 연산<br>$$ \text{dst} = \text{blackhat}(\text{src}, \text{element}) = \text{close}(\text{src}, \text{element}) - \text{src} $$ |
| `MorphTypes.HitMiss` | 히트미스 연산<br> `CV_8UC1` 형식의 이진 이미지만 가능 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.MORPH_DILATE` | 팽창 연산 |
| `cv2.MORPH_ERODE` | 침식 연산 |
| `cv2.MORPH_OPEN` | 열림 연산<br>$$ \text{dst} = \text{open}(\text{src}, \text{element}) = \text{dilate}(\text{erode}(\text{src}, \text{element})) $$ |
| `cv2.MORPH_CLOSE` | 닫힘 연산<br>$$ \text{dst} = \text{close}(\text{src}, \text{element}) = \text{erode}(\text{dilate}(\text{src}, \text{element})) $$ |
| `cv2.MORPH_GRADIENT` | 그라디언트 연산<br>$$ \text{dst} = \text{gradient}(\text{src}, \text{element}) = \text{dilate}(\text{src}, \text{element}) - \text{erode}(\text{src}, \text{element}) $$  |
| `cv2.MORPH_TOPHAT` | 탑 햇 연산<br>$$ \text{dst} = \text{tophat}(\text{src}, \text{element}) = \text{src} - \text{open}(\text{src}, \text{element}) $$ |
| `cv2.MORPH_BLACKHAT` | 블랙 햇 연산<br>$$ \text{dst} = \text{blackhat}(\text{src}, \text{element}) = \text{close}(\text{src}, \text{element}) - \text{src} $$ |
| `cv2.MORPH_HITMISS` | 히트미스 연산<br> `CV_8UC1` 형식의 이진 이미지만 가능 |

</div>
</div>

<br>

### 요약(Summary)

> 모폴로지 연산 방식을 설정합니다.
