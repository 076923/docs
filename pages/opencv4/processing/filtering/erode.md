---
title: 침식
sidebar: opencv4_sidebar
permalink: erode
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">dilate</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::erode(
    Mat src,
    Mat dst,
    Mat kernel,
    Point anchor = Point(-1,-1),
    int iterations = 1,
    int borderType = BORDER_CONSTANT,
    const Scalar& borderValue = morphologyDefaultBorderValue()
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Erode(
    Mat src,
    Mat dst, 
    Mat element,
    Point? anchor = null,
    int iterations = 1,
    BorderTypes borderType = BorderTypes.Constant,
    Scalar? borderValue = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.erode(
    src, 
    kernel,
    anchor = None,
    iterations = None,
    borderType = None,
    borderValue = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<b>침식(Erosion)</b>은 커널 영역 안에 존재하는 모든 픽셀의 값을 커널 내부의 <b>극솟값(Local Minimum)</b>으로 대체합니다.
{{site.data.alerts.end}}

{{site.data.alerts.note}}
침식 연산을 적용하면 <b>밝은 영역이 줄어들고 어두운 영역이 늘어납니다.</b> 커널의 크기나 반복 횟수에 따라 어두운 영역이 늘어나 <b>스펙클(Speckle)</b>이 사라지며 객체 내부의 <b>홀(Holes)</b>이 커집니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">고정점(anchor)</font>에 <font color="#c7254e">null</font> 값이나 <font color="#c7254e">None</font> 값을 사용하면 고정점의 위치는 <font color="#c7254e">(-1, -1)</font>을 갖게 됩니다.<br>
<li class="alerts_li"><font color="#c7254e">(-1, -1)</font>은 <b>커널의 중심부</b>를 의미합니다.</li>
{{site.data.alerts.end}}

<blockquote class="formula">
<b>침식 계산식(Erosion Formula):</b>
$$ \text{dst}(x,\ y) = \min _{(i,\ j) \ \in \ \text{kernel}} \text{src} (x+i,\ y+j) $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 침식 효과를 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 침식 효과를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 침식 효과가 적용된 이미지

> [`커널(kernel)`](getStructuringElement) 침식 효과를 적용하려는 구조 요소

> `고정점(anchor)` 콘벌루션(convolution) 연산을 적용하려는 지점

> `반복 횟수(iterations)` 침식 연산 반복 횟수

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

> `외삽 색상(borderValue)` 외삽된 픽셀의 색상

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 침식 효과가 적용된 이미지