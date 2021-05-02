---
title: 이진화 플래그
sidebar: opencv4_sidebar
permalink: ThresholdTypes
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
| `THRESH_BINARY` | $$ dst(x, y) = \begin{cases} \text{maxval} & \text{if:} \ src(x, y) > \text{thresh} \\ 0 & \text{else: otherwise} \end{cases} $$ |
| `THRESH_BINARY_INV` | $$ dst(x, y) = \begin{cases} 0 & \text{if:} \ src(x, y) > \text{thresh} \\ \text{maxval} & \text{else: otherwise} \end{cases} $$ |
| `THRESH_TRUNC` | $$ dst(x, y) = \begin{cases} \text{threshold} & \text{if:} \ src(x, y) > \text{thresh} \\ src(x, y) & \text{else: otherwise} \end{cases} $$ |
| `THRESH_TOZERO` | $$ dst(x, y) = \begin{cases} src(x, y) & \text{if:} \ src(x, y) > \text{thresh} \\ 0 & \text{else: otherwise} \end{cases} $$ |
| `THRESH_TOZERO_INV` | $$ dst(x, y) = \begin{cases} 0 & \text{if:} \ src(x, y) > \text{thresh} \\ src(x, y) & \text{else: otherwise} \end{cases} $$ |
| `THRESH_MASK` | 마스크용 이미지로 변경 |
| `THRESH_OTSU` | 오츠 알고리즘(Otsu Algorithm)을 적용하여 최적의 임곗값 계산 |
| `THRESH_TRIANGLE` | 삼각형 알고리즘(Triangle Algorithm)을 적용하여 최적의 임곗값 계산 |

<table style="margin-top: 4em;">
    <thead>
    <tr>
        <th style="text-align: center">연산</th>
        <th style="text-align: center">그래프</th>
        <th style="text-align: center">연산</th>
        <th style="text-align: center">그래프</th>
    </tr>
    </thead>
    <tbody>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">Source</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/src.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">Trunc</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/trunc.png" class="center_img"></td>
    </tr>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">Binary</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/binary.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">Tozero</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/tozero.png" class="center_img"></td>
    </tr>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">BinaryInv</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/binary_inv.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">TozeroInv</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/tozero_inv.png" class="center_img"></td>
    </tr>
    </tbody>
</table>

</div>

<div role="tabpanel" class="tab-pane" id="L2" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `ThresholdTypes.Binary` | $$ dst(x, y) = \begin{cases} \text{maxval} & \text{if:} \ src(x, y) > \text{thresh} \\ 0 & \text{else: otherwise} \end{cases} $$ |
| `ThresholdTypes.BinaryInv` | $$ dst(x, y) = \begin{cases} 0 & \text{if:} \ src(x, y) > \text{thresh} \\ \text{maxval} & \text{else: otherwise} \end{cases} $$ |
| `ThresholdTypes.Trunc` | $$ dst(x, y) = \begin{cases} \text{threshold} & \text{if:} \ src(x, y) > \text{thresh} \\ src(x, y) & \text{else: otherwise} \end{cases} $$ |
| `ThresholdTypes.Tozero` | $$ dst(x, y) = \begin{cases} src(x, y) & \text{if:} \ src(x, y) > \text{thresh} \\ 0 & \text{else: otherwise} \end{cases} $$ |
| `ThresholdTypes.TozeroInv` | $$ dst(x, y) = \begin{cases} 0 & \text{if:} \ src(x, y) > \text{thresh} \\ src(x, y) & \text{else: otherwise} \end{cases} $$ |
| `ThresholdTypes.Mask` | 마스크용 이미지로 변경 |
| `ThresholdTypes.Otsu` | 오츠 알고리즘(Otsu Algorithm)을 적용하여 최적의 임곗값 계산 |
| `ThresholdTypes.Triangle` | 삼각형 알고리즘(Triangle Algorithm)을 적용하여 최적의 임곗값 계산 |

<table style="margin-top: 4em;">
    <thead>
    <tr>
        <th style="text-align: center">연산</th>
        <th style="text-align: center">그래프</th>
        <th style="text-align: center">연산</th>
        <th style="text-align: center">그래프</th>
    </tr>
    </thead>
    <tbody>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">Source</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/src.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">Trunc</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/trunc.png" class="center_img"></td>
    </tr>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">Binary</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/binary.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">Tozero</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/tozero.png" class="center_img"></td>
    </tr>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">BinaryInv</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/binary_inv.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">TozeroInv</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/tozero_inv.png" class="center_img"></td>
    </tr>
    </tbody>
</table>

</div>

<div role="tabpanel" class="tab-pane" id="L3" markdown="1">

| 플래그             | 설명                                                             |
| ----------------- | ---------------------------------------------------------------- | 
| `cv2.THRESH_BINARY` | $$ dst(x, y) = \begin{cases} \text{maxval} & \text{if:} \ src(x, y) > \text{thresh} \\ 0 & \text{else: otherwise} \end{cases} $$ |
| `cv2.THRESH_BINARY_INV` | $$ dst(x, y) = \begin{cases} 0 & \text{if:} \ src(x, y) > \text{thresh} \\ \text{maxval} & \text{else: otherwise} \end{cases} $$ |
| `cv2.THRESH_TRUNC` | $$ dst(x, y) = \begin{cases} \text{threshold} & \text{if:} \ src(x, y) > \text{thresh} \\ src(x, y) & \text{else: otherwise} \end{cases} $$ |
| `cv2.THRESH_TOZERO` | $$ dst(x, y) = \begin{cases} src(x, y) & \text{if:} \ src(x, y) > \text{thresh} \\ 0 & \text{else: otherwise} \end{cases} $$ |
| `cv2.THRESH_TOZERO_INV` | $$ dst(x, y) = \begin{cases} 0 & \text{if:} \ src(x, y) > \text{thresh} \\ src(x, y) & \text{else: otherwise} \end{cases} $$ |
| `cv2.THRESH_MASK` | 마스크용 이미지로 변경 |
| `cv2.THRESH_OTSU` | 오츠 알고리즘(Otsu Algorithm)을 적용하여 최적의 임곗값 계산 |
| `cv2.THRESH_TRIANGLE` | 삼각형 알고리즘(Triangle Algorithm)을 적용하여 최적의 임곗값 계산 |

<table style="margin-top: 4em;">
    <thead>
    <tr>
        <th style="text-align: center">연산</th>
        <th style="text-align: center">그래프</th>
        <th style="text-align: center">연산</th>
        <th style="text-align: center">그래프</th>
    </tr>
    </thead>
    <tbody>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">Source</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/src.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">Trunc</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/trunc.png" class="center_img"></td>
    </tr>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">Binary</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/binary.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">Tozero</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/tozero.png" class="center_img"></td>
    </tr>
    <tr style="background-color: white;">
        <td style="text-align: center"><code class="highlighter-rouge">BinaryInv</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/binary_inv.png" class="center_img"></td>
        <td style="text-align: center"><code class="highlighter-rouge">TozeroInv</code></td>
        <td style="text-align: center"><img src="images/opencv4/ThresholdTypes/tozero_inv.png" class="center_img"></td>
    </tr>
    </tbody>
</table>

</div>
</div>

<br>

### 요약(Summary)

> 이진화 계산 방식을 설정합니다.
