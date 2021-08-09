---
title: 샤르
sidebar: opencv4_sidebar
permalink: Scharr
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">Scharr</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::Scharr(
    Mat src,
    Mat dst,
    int ddepth,
    int dx,
    int dy,
    double scale = 1,
    double delta = 0,
    int borderType = BORDER_DEFAULT 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Scharr(
    Mat src,
    Mat dst,
    MatType ddepth,
    int xorder, 
    int yorder,
    double scale = 1,
    double delta = 0,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.Scharr(
    src,
    ddepth,
    dx,
    dy,
    scale = None,
    delta = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
샤르는 3x3 크기만 지원하며, 소벨보다 더 빠르고 정확하기 때문에 3×3 필터를 사용한다면 샤르를 활용합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>샤르 계산식(Scharr Formula):</b>
$$ \text{dst} = \frac{\partial^{xorder+yorder} \text{src}}{\partial x^{xorder} \partial y^{yorder}} $$
<b>방향에 따른 필터 형태(Filter type according to direction):</b>
$$ \begin{matrix}
\begin{bmatrix}
-3 & 0 & 3 \\ 
-10 & 0 & 10 \\ 
-3 & 0 & 3
\end{bmatrix} & \begin{bmatrix}
-3 & -10 & -3 \\ 
0 & 0 & 0 \\ 
3 & 10 & 3
\end{bmatrix} \\ 
\ 3 \times 3 \ \text{Vertical Mask} & 3 \times 3 \  \text{HorizontalMask}
\end{matrix} $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 X축과 Y축을 따라 1차 미분 값을 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 샤르를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 샤르가 적용된 이미지

> `출력 이미지 정밀도(ddepth)` 출력 이미지의 정밀도 설정

> `X 방향 차수(dx, xorder)` X축 미분 차수

> `Y 방향 차수(dy, yorder)` Y축 미분 차수

> `비율(scale)` 필터링 된 픽셀에 곱해지는 값

> `오프셋(delta)` 필터링 된 픽셀에 더해지는 값

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 샤르가 적용된 이미지