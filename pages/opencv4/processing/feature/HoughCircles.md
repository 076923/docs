---
title: 허프 원 변환
sidebar: opencv4_sidebar
permalink: HoughCircles
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">HoughCircles</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::HoughCircles(
    Mat image,
    Mat circles,
    int method,
    double dp,
    double minDist,
    double param1 = 100,
    double param2 = 100,
    int minRadius = 0,
    int maxRadius = 0 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">CircleSegment[] Cv2.HoughCircles(
    Mat image,
    HoughModes method,
    double dp,
    double minDist,
    double param1 = 100
    double param2 = 100,
    int minRadius = 0,
    int maxRadius = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">circles = cv2.HoughCircles(
    image,
    method,
    dp,
    minDist,
    circles = None,
    double param1 = None
    double param2 = None,
    int minRadius = None,
    int maxRadius = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
허프 원 검출은 소벨 엣지를 통해 x, y에 대한 1차 소벨 도함수를 계산해서 그레이디언트를 구하는 <font color="#c7254e">그레이디언트(Gradient)</font> 방법과 히스토그램에 필요한 메모리가 줄여 계산하는 <font color="#c7254e">2단계 허프 변환(Two stage Hough Transform)</font> 방법을 활용해 원을 검출합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">입력 이미지(src)</font>는 <b>단일 채널 8 비트</b> 형식 이미지를 사용합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지에 허프 원 검출을 실행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 허프 원 검출을 계산하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}">원(circles)</a> 검출된 원의 중심점 및 반지름

> `검출 방법(method)` 2단계 허프 변환 방법

> `해상도 비율(dp)` 누산 평면의 해상도

> `최소 거리(minDist)` 일차적으로 검출된 원과 원 사이의 최소 거리

> `캐니 엣지 임곗값(param1)` 캐니 엣지의 상위 임곗값

> `중심 임곗값(param2)` 그레이디언트 방법에 적용된 중심 히스토그램(누산 평면)에 대한 임곗값

> `최소 반지름(minRadius)` 검출될 원의 최소 반지름

> `최대 반지름(maxRadius)` 검출될 원의 최대 반지름

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS_Python}}">원(circles)</a> 검출된 원의 중심점 및 반지름