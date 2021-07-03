---
title: 아핀 변환 행렬 반환
sidebar: opencv4_sidebar
permalink: getAffineTransform
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getAffineTransform</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat cv::getAffineTransform(
    const Point2f src[],
    const Point2f dst[]
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.GetAffineTransform(
    IEnumerable&lt;Point2f&gt; src,
    IEnumerable&lt;Point2f&gt; dst
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getAffineTransform(
    src,
    dst
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
실제 아핀 변환 행렬은 <b>3×3</b>이며, OpenCV에서는 불필요한 연산을 줄이기 위해 <b>2×3</b> 행렬로 표현합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>아핀 변환 행렬 계산식(Affine Transform Matrix Formula):</b>
$$ \begin{bmatrix} {x_1}' \\ {y_1}' \\ {x_2}' \\ {y_2}' \\ {x_3}' \\ {y_3}' \\ \end{bmatrix} = \begin{bmatrix} {x_1} & {y_1} & 0 & 0 & 1 & 0 \\ 0 & 0 & {x_1} & {y_1} & 0 & 1 \\ {x_2} & {y_2} & 0 & 0 & 1 & 0 \\ 0 & 0 & {x_2} & {y_2} & 0 & 1 \\ {x_3} & {y_3} & 0 & 0 & 1 & 0 \\ 0 & 0 & {x_3} & {y_3} & 0 & 1 \\ \end{bmatrix} \cdot \begin{bmatrix} a \\ b \\ c \\ d \\ e \\ f \\ \end{bmatrix} $$
</blockquote>

<blockquote class="formula">
<b>아핀 변환 행렬(Affine Transform Matrix):</b>
$$ \text{matrix} = \begin{bmatrix} a & b & e \\ c & d & f \\ 0 & 0 & 1 \end{bmatrix} \Rightarrow \begin{bmatrix} a & b & e \\ c & d & f \end{bmatrix} $$
</blockquote>

<br>

### 요약(Summary)

> 여섯 개의 좌표를 활용해 아핀 변환 행렬을 생성합니다.

### 매개변수(Parameter)

> `변환 전 세 개의 픽셀 좌표(src)` 아핀 변환 행렬 생성을 위한 삼각형 형태의 픽셀 기준 좌표

> `변환 후 세 개의 픽셀 좌표(dst)` 아핀 변환 행렬 생성을 위한 삼각형 형태의 픽셀 기준 좌표

### 반환값(Returns)

> `아핀 변환 행렬(retval)` 2×3 아핀 변환 행렬