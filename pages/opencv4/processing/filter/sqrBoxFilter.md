---
title: 제곱합 박스 필터
sidebar: opencv4_sidebar
permalink: sqrBoxFilter
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">sqrBoxFilter</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::sqrBoxFilter(
	Mat src,
    Mat dst,
    int ddepth,
    Size ksize,
    Point anchor = Point(-1, -1),
    bool normalize = true,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.SqrBoxFilter(
    Mat src,
    Mat dst,
    int ddepth,
    Size ksize,
    Point? anchor = null,
    bool normalize = true,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.sqrBoxFilter(
    src,
    ddepth, 
    ksize,
    anchor = None,
    normalize = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
필터와 중복되는 픽셀의 제곱합을 계산합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">고정점(anchor)</font>에 <font color="#c7254e">null</font> 값이나 <font color="#c7254e">None</font> 값을 사용하면 고정점의 위치는 <font color="#c7254e">(-1, -1)</font>을 갖게 됩니다.<br>
<li class="alerts_li"><font color="#c7254e">(-1, -1)</font>은 <b>커널의 중심부</b>를 의미합니다.</li>
{{site.data.alerts.end}}

{{site.data.alerts.important}}
<font color="#c7254e">정규화(normalize)</font>를 하지 않는 경우, 픽셀 주변의 <b>분산</b> 및 <b>표준 편차</b>를 계산할 수 있습니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지에 제곱합 박스 필터를 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 제곱합 박스 필터를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 제곱합 박스 필터가 적용된 이미지

> `출력 이미지 정밀도(ddepth)` 출력 이미지의 정밀도 설정

> `커널 크기(ksize)` 커널의 크기(너비, 높이)

> `고정점(anchor)` 콘벌루션(convolution) 연산을 적용하려는 지점

> `정규화(normalize)` 박스 필터의 정규화 유/무

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 제곱합 박스 필터가 적용된 이미지