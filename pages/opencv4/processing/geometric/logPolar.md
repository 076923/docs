---
title: 로그 매핑
sidebar: opencv4_sidebar
permalink: logPolar
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">logPolar</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::logPolar(
    Mat src,
    Mat dst,
    Point2f center,
    double M,
    int flags 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.LogPolar(
    Mat src,
    Mat dst,
    Point2f center,
    double m,
    InterpolationFlags flags
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.logPolar(
    src,
    center,
    M,
    flags
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 이미지를 로그 극좌표 공간에 매핑합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 로그 극좌표 공간으로 매핑하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 로그 극좌표 공간으로 매핑된 출력 이미지

> `중심점(center)` 매핑 기준점

> `크기(m)` 변형하려는 크기(magnitude) 비율

> [`내삽 방식(flags)`](InterpolationFlags) 이미지 내의 픽셀을 내삽하는데 사용되는 계산 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 로그 극좌표 공간으로 매핑된 출력 이미지
