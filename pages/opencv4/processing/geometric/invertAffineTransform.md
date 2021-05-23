---
title: 아핀 변환 역행렬 반환
sidebar: opencv4_sidebar
permalink: invertAffineTransform
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">invertAffineTransform</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::invertAffineTransform(
    Mat M,
    Mat iM
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.InvertAffineTransform(
    Mat m,
    Mat im
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">iM = cv2.invertAffineTransform(
    M
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
실제 아핀 변환 행렬은 <b>3×3</b>이며, OpenCV에서는 불필요한 연산을 줄이기 위해 <b>2×3</b> 행렬로 표현합니다.
{{site.data.alerts.end}}

{% include callout.html content="
`아핀 변환 역행렬(invert matrix)`
<br><br>
$$ invert\ matrix=\begin{bmatrix} a_{11} & a_{12} & b_{1} \\ a_{21} & a_{22} & b_{2} \\ 0 & 0 & 1 \end{bmatrix}^{-1} $$
" type="success" %}

<br>

### 요약(Summary)

> 아핀 변환 행렬의 역을 계산합니다.

### 매개변수(Parameter)

> `아핀 변환 행렬(M)` 2×3 아핀 변환 행렬

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">아핀 변환 역행렬(iM)</a> 2×3 아핀 변환 역행렬

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">아핀 변환 역행렬(iM)</a> 2×3 아핀 변환 역행렬
