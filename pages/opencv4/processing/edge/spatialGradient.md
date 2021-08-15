---
title: 공간 그라디언트
sidebar: opencv4_sidebar
permalink: spatialGradient
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">spatialGradient</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::spatialGradient(
    Mat src,
    Mat dx,
    Mat dy,
    int ksize = 3,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.SpatialGradient(
    InputArray src, OutputArray dx, OutputArray dy, int ksize = 3, BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.spatialGradient(
    src,
    ddepth,
    dx,
    dy,
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
<a herf="Sobel">소벨(Sobel)</a>을 활용해 인접한 픽셀들의 차이로 <b>기울기(Gradient)</b>의 크기를 계산합니다.
{{site.data.alerts.end}}

{{site.data.alerts.important}}
<font color="#c7254e">공간 그라디언트 출력 이미지(dx, dy)</font>는 <font color="#c7254e">CV_16SC1</font> 형식으로 반환됩니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지의 X축과 Y축에 따라 1차 미분한 값을 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 공간 그라디언트를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">X 방향 출력 이미지(dx)</a> X축 공간 그라디언트 적용된 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">Y 방향 출력 이미지(dy)</a> Y축 공간 그라디언트 적용된 이미지

> `커널 크기(ksize)` 커널의 크기

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">X 방향 출력 이미지(dx)</a> Y축 공간 그라디언트 적용된 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">Y 방향 출력 이미지(dy)</a> Y축 공간 그라디언트 적용된 이미지