---
title: 라플라시안
sidebar: opencv4_sidebar
permalink: Laplacian
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">Laplacian</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::Laplacian(
    Mat src,
    Mat dst,
    int ddepth,
    int ksize = 1,
    double scale = 1,
    double delta = 0,
    int borderType = BORDER_DEFAULT 
)		
</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Laplacian(
    Mat src,
    Mat dst,
    MatType ddepth,
    int ksize = 1,
    double scale = 1,
    double delta = 0,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.Laplacian(
    src,
    ddepth
    ksize = None,
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
가장자리가 밝은 부분에서 발생한 것인지, 어두운 부분에서 발생한 것인지 확인할 수 있습니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>라플라시안 계산식(Laplacian Formula):</b>
$$ \text{dst} = \Delta \text{src} = \frac{\partial^2 \text{src}}{\partial x^2} + \frac{\partial^2 \text{src}}{\partial y^2} $$
<b>커널 크기에 따른 필터 형태(Filter type according to kernel size):</b>
$$ \text{kernel} = \begin{bmatrix}
0 & 1 & 0 \\ 
1 & -4 & 1 \\ 
0 & 1 & 0
\end{bmatrix}
\text{if:} \ \text{ksize} == 1 $$
$$ \text{kernel} = \begin{bmatrix}
-1 & -1 & -1 \\ 
-1 & 8 & -1 \\ 
-1 & -1 & -1
\end{bmatrix}
\text{if:} \ \text{ksize} > 1 $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 x축과 y축을 따라 2차 미분한 합을 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 라플라시안을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 라플라시안이 적용된 이미지

> `출력 이미지 정밀도(ddepth)` 출력 이미지의 정밀도 설정

> `커널 크기(ksize)` 커널의 크기(너비, 높이)

> `비율(scale)` 필터링 된 픽셀에 곱해지는 값

> `오프셋(delta)` 필터링 된 픽셀에 더해지는 값

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 라플라시안이 적용된 이미지