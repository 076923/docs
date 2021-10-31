---
title: 점진성 확률적 허프 선 변환
sidebar: opencv4_sidebar
permalink: HoughLinesP
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">HoughLinesP</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::HoughLinesP(
    Mat image,
    Mat lines,
    double rho,
    double theta,
    int threshold,
    double minLineLength = 0,
    double maxLineGap = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">LineSegmentPoint[] Cv2.HoughLines(
    Mat image,
    double rho,
    double theta,
    int threshold,
    double minLineLength = 0,
    double maxLineGap = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">lines = cv2.HoughLinesP(
    image,
    rho,
    theta,
    threshold,
    minLineLength = None,
    maxLineGap = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
점진성 확률적 허프 선 변환은 <b>모든 점을 대상으로 직선의 방정식을 세우는 것이 아닌, 임의의 점 일부만 누적해서 계산합니다.</b>
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">입력 이미지(src)</font>는 <b>단일 채널 8 비트</b> 형식 이미지를 사용합니다.<br>
<font color="#c7254e">거리(rho)</font>의 단위는 픽셀을 의미하며, <b>0.0 ~ 1.0</b>의 실수 범위를 갖습니다.<br>
<font color="#c7254e">각도(theta)</font>는 라디안 단위로 <b>0 ~ 180</b>의 범위를 갖습니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지에 점진성 확률적 허프 선 변환을 실행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 점진성 확률적 허프 선 변환을 계산하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}">선(lines)</a> 검출된 선의 시작점(P1)과 도착점(P2)

> `거리(rho)` 누산 평면에서 사용되는 거리에 대한 분해능

> `각도(theta)` 누산 평면에서 사용되는 각도에 대한 분해능

> `임곗값(threshold)` 직선을 결정하기 위해 만족해야 하는 누산 평면의 값

> `최소 선 길이(minLineLength)` 검출된 직선이 가져야 하는 최소한의 길이

> `최대 선 간격(maxLineGap)` 검출된 직선들 사이의 최대 허용 간격

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS_Python}}">선(lines)</a> 검출된 선의 시작점(P1)과 도착점(P2)