---
title: 해리스 코너 검출
sidebar: opencv4_sidebar
permalink: cornerHarris
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">cornerHarris</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::cornerHarris(
    Mat src,
    Mat dst,
    int blockSize,
    int ksize,
    double k,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.CornerHarris(
    Mat src,
    Mat dst,
    int blockSize,
    int ksize,
    double k,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.cornerHarris(
    src,
    blockSize,
    ksize,
    k,
    dst = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
각 <b>픽셀(x, y)</b>에 대해 <font color="#c7254e">블록 크기(blockSize)</b> 이웃(Neighborhood)에 대한 2 × 2 기울기 공분산 행렬 <b>M(x, y)</b>를 계산합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">입력 이미지(src)</font>는 <b>단일 채널 8 비트</b> 형식 이미지를 사용하거나, <b>부동 소수점</b> 형식 이미지를 사용합니다.<br>
<font color="#c7254e">출력 이미지(dst)</font>는 <font color="#c7254e">CV_32FC1</font> 형식을 반환합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>해리스 코너 특성 계산식(Harris Corner Characteristic Formula):</b>
$$ \text{dst}(x,\ y) = \mathrm{det} M^{(x,\ y)} - k \cdot \left ( \mathrm{tr} M^{(x,\ y)} \right )^2 $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 해리스 코너 감지기를 실행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 해리스 코너를 계산하려는 입력 이미지

> `출력 이미지(dst)` 해리스 코너가 계산된 이미지

> `블록 크기(blockSize)` 이웃(Neighborhood)의 크기

> `커널 크기(ksize)` 소벨(Sobel) 커널의 크기

> `해리스 측정 계수(K)` 해리스 코너 특성 계산식의 k 계수

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 해리스 코너가 계산된 이미지