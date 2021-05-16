---
title: 원근 변환 행렬 생성
sidebar: opencv4_sidebar
permalink: getPerspectiveTransform
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getPerspectiveTransform</h2>
    </div>
    <div class="col-lg-12">

        <ul id="myTab" class="nav nav-tabs nav-justified">
            <li class="active"><a href="#service-one" data-toggle="tab"><i class="fa fa-support"></i> C++</a>
            </li>
            <li class=""><a href="#service-two" data-toggle="tab"><i class="fa fa-support"></i> C#</a>
            </li>
            <li class=""><a href="#service-three" data-toggle="tab"><i class="fa fa-support"></i> Python</a>
            </li>
        </ul>

        <div id="myTabContent" class="tab-content">
            <div class="tab-pane fade active in" id="service-one">
<pre class="prettyprint"><code class="language-cpp">Mat cv::getPerspectiveTransform(
    const Point2f src[],
    const Point2f dst[],
    int solveMethod = DECOMP_LU
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.GetPerspectiveTransform(
    IEnumerable&lt;Point2f&gt; src,
    IEnumerable&lt;Point2f&gt; dst
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getPerspectiveTransform(
    src,
    dst,
    solveMethod = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="
`원근 변환 행렬 계산식(Affine Transform Matrix Formula)`
<br><br>
$$ \begin{bmatrix} {x_1}' \\ {y_1}' \\ {x_2}' \\ {y_2}' \\ {x_3}' \\ {y_3}' \\ {x_4}' \\ {y_4}' \end{bmatrix} = \begin{bmatrix} {x_1} & {y_1} & 1 & 0 & 0 & 0 & -{x_1}' \cdot {x_1} & -{x_1}' \cdot {y_1} \\ 0 & 0 & 0 & {x_1} & {y_1} & 1 & -{y_1}' \cdot {x_1} & -{y_1}' \cdot {y_1} \\ {x_2} & {y_2} & 1 & 0 & 0 & 0 & -{x_2}' \cdot {x_2} & -{x_2}' \cdot {y_2} \\ 0 & 0 & 0 & {x_2} & {y_2} & 1 & -{y_2}' \cdot {x_2} & -{y_2}' \cdot {y_2} \\ {x_3} & {y_3} & 1 & 0 & 0 & 0 & -{x_3}' \cdot {x_3} & -{x_3}' \cdot {y_3} \\ 0 & 0 & 0 & {x_3} & {y_3} & 1 & -{y_3}' \cdot {x_3} & -{y_3}' \cdot {y_3} \\ {x_4} & {y_4} & 1 & 0 & 0 & 0 & -{x_4}' \cdot {x_4} & -{x_4}' \cdot {y_4} \\ 0 & 0 & 0 & {x_4} & {y_4} & 1 & -{y_4}' \cdot {x_4} & -{y_4}' \cdot {y_4} \\ \end{bmatrix} \cdot \begin{bmatrix} a \\ b \\ c \\ d \\ e \\ f \\ g \\ h \end{bmatrix} $$
<br><br>
`원근 변환 행렬(Perspective Transform Matrix)`
<br><br>
$$ \text{matrix} = \begin{bmatrix} a & b & e \\ c & d & f \\ g & h & 1 \end{bmatrix} $$

" type="success" %}

<br>

### 요약(Summary)

> 여덟 개의 좌표를 활용해 원근 변환 행렬을 생성합니다.

### 매개변수(Parameter)

> `변환 전 네 개의 픽셀 좌표(src)` 원근 변환 행렬 생성을 위한 사각형 형태의 픽셀 기준 좌표

> `변환 후 네 개의 픽셀 좌표(dst)` 원근 변환 행렬 생성을 위한 사각형 형태의 픽셀 기준 좌표

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}" href="DecompTypes" style="cursor: revert;">행렬 분해 방식(solveMethod)</a> 원근 변환 행렬 분해 계산 방식

### 반환값(Returns)

> `원근 변환 행렬(retval)` 3×3 원근 변환 행렬