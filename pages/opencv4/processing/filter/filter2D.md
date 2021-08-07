---
title: 2D 필터
sidebar: opencv4_sidebar
permalink: filter2D
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">filter2D</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::filter2D(
    Mat src,
    Mat dst,
    int ddepth,
    Mat kernel,
    Point anchor = Point(-1,-1),
    double delta = 0,
    int borderType = BORDER_DEFAULT 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Filter2D(
    Mat src,
    Mat dst,
    MatType ddepth,
    Mat kernel,
    Point? anchor = null,
    double delta = 0,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.filter2D(
    src,
    ddepth,
    kernel,
    anchor = None,
    delta = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
2D 필터는 <font color="#c7254e">콘벌루션(convolution)</font> 연산이 아닌 <font color="#c7254e">상관관계(correlation)</font>를 계산합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">커널(Kernel)</font>이 11 × 11 보다 큰 경우에는 <b>이산 푸리에 변환(Discrete Fourier Transform)</b> 알고리즘을 사용하며, 11 × 11 보다 작은 경우에는 <b>다이렉트(DIRECT)</b> 알고리즘을 사용합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>팽창 계산식(Dilation Formula):</b>
$$ \text{dst} (x,\ y) = \sum_{ \substack{ 0\leq x' < \text{kernel.cols} \\ {0\leq y' < \text{kernel.rows}}}} \text{kernel} (x',\ y') \cdot \text{src} (x+x'- \text{anchor}.x, \ y+y'- \text{anchor}.y) $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 임의의 선형 필터를 이미지에 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 임의의 선형 필터를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 임의의 선형 필터가 적용된 이미지

> `출력 이미지 정밀도(ddepth)` 출력 이미지의 정밀도 설정

> `커널(kernel)` 임의의 선형 필터를 적용하려는 단일 채널 부동 소수점 행렬

> `고정점(anchor)` 필터의 상대적 위치를 나타내는 커널의 중심부

> `오프셋(delta)` 필터링 된 픽셀에 더해지는 값

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 임의의 선형 필터가 적용된 이미지