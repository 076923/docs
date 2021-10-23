---
title: 표준 / 멀티 스케일 허프 선 변환
sidebar: opencv4_sidebar
permalink: HoughLines
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">HoughLines</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::HoughLines(
    Mat image,
    Mat lines,
    double rho,
    double theta,
    int threshold,
    double srn = 0,
    double stn = 0,
    double min_theta = 0,
    double max_theta = CV_PI
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">LineSegmentPolar[] Cv2.HoughLines(
    Mat image,
    double rho,
    double theta,
    int threshold,
    double srn = 0,
    double stn = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">lines = cv2.HoughLines(
    image,
    rho,
    theta,
    threshold,
    lines = None,
    srn = None,
    stn = None,
    min_theta = None,
    max_theta = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
허프 선 변환은 <b>이미지 내의 어떤 점이라도 선 집합의 일부일 수 있다</b>는 가정하에 직선의 방정식을 이용해 직선을 검출합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">입력 이미지(src)</font>는 <b>단일 채널 8 비트</b> 형식 이미지를 사용합니다.<br>
<font color="#c7254e">거리(rho)</font>의 단위는 픽셀을 의미하며, <b>0.0 ~ 1.0</b>의 실수 범위를 갖습니다.<br>
<font color="#c7254e">각도(theta)</font>는 라디안 단위로 <b>0 ~ 180</b>의 범위를 갖습니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">거리 약수(srn)</font>와 <font color="#c7254e">각도 약수(stn)</font>가 모두 0인 경우, <b>표준 허프 변환</b>이 적용됩니다.<br>
<font color="#c7254e">거리 약수(srn)</font>와 <font color="#c7254e">각도 약수(stn)</font>가 모두 0이 아니라면, <b>멀티 스케일 허프 변환</b>이 적용됩니다. 
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지에 허프 선 변환을 실행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 허프 선 변환을 계산하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}">선(lines)</a> 검출된 선의 거리(rho)와 각도(theta)

> `거리(rho)` 누산 평면에서 사용되는 거리에 대한 해상도

> `각도(theta)` 누산 평면에서 사용되는 각도에 대한 해상도

> `임곗값(threshold)` 직선을 결정하기 위해 만족해야 하는 누산 평면의 값

> `거리 약수(srn)` 거리(rho)에 대한 약수(divisor)

> `각도 약수(stn)` 거리(theta)에 대한 약수(divisor)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}">최소 각도(min_theta)</a> 직선의 최소 각도

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}">최대 각도(max_theta)</a> 직선의 최대 각도

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS_Python}}">선(lines)</a> 검출된 선의 거리(rho)와 각도(theta)