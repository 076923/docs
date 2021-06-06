---
title: 회전 변환 행렬 반환
sidebar: opencv4_sidebar
permalink: getRotationMatrix2D
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getRotationMatrix2D</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat cv::getRotationMatrix2D(
    Point2f center,
    double angle,
    double scale
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.GetRotationMatrix2D(
    Point2f center,
    double angle,
    double scale
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getRectSubPix(
    center,
    angle,
    scale
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
회전 변환 행렬은 <b>중심점(center)</b>을 기준으로 행렬을 계산합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `각도(angle)`는 도(°) 단위와 반시계 방향을 갖습니다.
  
- `회전 변환 행렬(matrix)` 부동 소수점 형태의 2×3 회전 변환 행렬을 반환합니다.

" type="success" %}

{% include callout.html content="
`회전 변환 행렬(matrix)`
<br><br>
$$ matrix = \begin{bmatrix} a & b & e \\ c & d & f \end{bmatrix} = \begin{bmatrix} \alpha & \beta & (1-\alpha) \cdot \text{center.}x - \beta \cdot \text{center.}y \\ -\beta & \alpha & \beta \cdot \text{center.}x + (1-\alpha) \cdot \text{center.}y \end{bmatrix} $$
<br><br>
$$ \alpha = \text{scale} \cdot \cos(\text{angle}) $$ &emsp; $$ \beta= \text{scale} \cdot \sin(\text{angle}) $$
" type="success" %}

<br>

### 요약(Summary)

> 2 차원 회전 아핀 변환 행렬을 계산합니다.

### 매개변수(Parameter)

> `중심점(center)` 회전하려는 이미지의 중심

> `각도(angle)` 회전하려는 이미지의 각도

> `비율(scale)` 회전하려는 이미지의 확대 또는 축소 비율

### 반환값(Returns)

> `회전 변환 행렬(matrix)` 2×3 회전 변환 행렬