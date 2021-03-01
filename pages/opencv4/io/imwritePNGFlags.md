---
title: PNG 형식 플래그
sidebar: opencv4_sidebar
permalink: imwritePNGFlags
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
| `IMWRITE_PNG_STRATEGY_DEFAULT` | 일반 데이터 값 적용 |
| `IMWRITE_PNG_STRATEGY_FILTERED` | 필터로 생성된 데이터 값 적용 |
| `IMWRITE_PNG_STRATEGY_HUFFMAN_ONLY` | 허프먼(Huffman) 부호화 적용 |
| `IMWRITE_PNG_STRATEGY_RLE` | 정합 거리 제한 |
| `IMWRITE_PNG_STRATEGY_FIXED` | 허프먼(Huffman) 부호화 방지 |


</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `ImwritePNGFlags.StrategyDefault` | 일반 데이터 값 적용 |
| `ImwritePNGFlags.StrategyFiltered` | 필터로 생성된 데이터 값 적용 |
| `ImwritePNGFlags.StrategyHuffmanOnly` | 허프먼(Huffman) 부호화 적용 |
| `ImwritePNGFlags.StrategyRLE` | 정합 거리 제한 |
| `ImwritePNGFlags.StrategyFixed` | 허프먼(Huffman) 부호화 방지 |

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.IMWRITE_PNG_STRATEGY_DEFAULT` | 일반 데이터 값 적용 |
| `cv2.IMWRITE_PNG_STRATEGY_FILTERED` | 필터로 생성된 데이터 값 적용 |
| `cv2.IMWRITE_PNG_STRATEGY_HUFFMAN_ONLY` | 허프먼(Huffman) 부호화 적용 |
| `cv2.IMWRITE_PNG_STRATEGY_RLE` | 정합 거리 제한 |
| `cv2.IMWRITE_PNG_STRATEGY_FIXED` | 허프먼(Huffman) 부호화 방지 |

</div>
</div>

### 요약(Summary)

> PNG 저장 방식을 설정합니다.