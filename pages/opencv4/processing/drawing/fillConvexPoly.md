---
title: 채워진 볼록 다각형 그리기    
sidebar: opencv4_sidebar
permalink: fillConvexPoly
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">fillConvexPoly</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::fillConvexPoly(
    Mat img,
    Mat points,
    const Scalar& color,
    int lineType = LINE_8,
    int shift = 0 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.FillConvexPoly(
    Mat img,
    IEnumerable&lt;Point&gt; pts,
    Scalar color,
    LineTypes lineType = LineTypes.Link8,
    int shift = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">img = cv2.fillConvexPoly(
    img,
    points,
    color,
    lineType = None,
    shift = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
입력 이미지에 그리기 함수를 직접 적용해 입력 이미지 자체가 변경됩니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">볼록(Convex)</font>한 영역에 대해서는 채워진 다각형을 그리며, 볼록하지 않은 영역에 대해서는 윤곽선만 그립니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 이미지에 윤곽선 영역 중 볼록(Convex)한 영역만 채워 그립니다.

### 매개변수(Parameter)

> `이미지(img)` 다각형을 그릴려는 이미지

> `윤곽선(points)` 그리려는 다각형

> `색상(color)` 다각형의 색상

> [`선형 타입(lineType)`](LineTypes) 선의 유형 설정

> `비트 시프트(shift)` 소수점 이하의 값이 포함된 실숫값 좌표로 그리기 위한 비트 수

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">이미지(img)</a> 다각형이 그려진 이미지