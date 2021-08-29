---
title: 호 윤곽선 반환
sidebar: opencv4_sidebar
permalink: ellipse2Poly
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">ellipse2Poly</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::ellipse2Poly(
    Point center,
    Size axes,
    int angle,
    int arcStart,
    int arcEnd,
    int delta,
    std::vector&lt;Point&gt;& pts 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Point[] Cv2.Ellipse2Poly(
    Point center,
    Size axes,
    int angle,
    int arcStart,
    int arcEnd,
    int delta
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">pts = cv2.ellipse2Poly(
    center,
    axes,
    angle,
    arcStart,
    arcEnd,
    delta
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 호나 타원을 윤곽선 형태로 반환합니다.

### 매개변수(Parameter)

> `중심점(center)` 호의 중심점

> `장축과 단축(axes)` 호의 장축과 단축

> `각도(angle)` 장축이 기울어진 각도

> `시작 각도(startAngle)` 호가 그려지는 시작 각도

> `도착 각도(endAngle)` 호가 그려지는 도착 각도

> `근사 정확도(delta)` 윤곽선 지점의 간격

> `지점(pts)` 호의 윤곽선 지점

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS_Python}}">지점(pts)</a> 호의 윤곽선 지점