---
title: 마커 그리기
sidebar: opencv4_sidebar
permalink: drawMarker
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">drawMarker</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::drawMarker(
    Mat img,
    Point position,
    const Scalar& color,
    int markerType = MARKER_CROSS,
    int markerSize = 20,
    int thickness = 1,
    int line_type = 8 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.DrawMarker(
    Mat img,
    Point position,
    Scalar color,
    MarkerTypes markerType = MarkerTypes.Cross,
    int markerSize = 20,
    int thickness = 1,
    LineTypes lineType = LineTypes.Link8
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">img = cv2.drawMarker(
    img,
    position,
    color,
    markerType,
    markerSize = None,
    thickness = None,
    line_type = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
입력 이미지에 그리기 함수를 직접 적용해 입력 이미지 자체가 변경됩니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 이미지에 특정 마커를 그립니다.

### 매개변수(Parameter)

> `이미지(img)` 마커를 그릴려는 이미지

> `위치(position)` 마커의 위치

> `색상(color)` 마커의 색상

> [`마커 모양(markerType)`](MarkerTypes) 마커의 형태

> `마커 크기(markerSize)` 마커의 크기

> `두께(thickness)` 마커의 두께

> [`선형 타입(line_type)`](LineTypes) 선의 유형 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">이미지(img)</a> 마커가 그려진 이미지