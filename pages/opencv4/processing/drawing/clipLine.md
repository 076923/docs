---
title: 직선 클리핑
sidebar: opencv4_sidebar
permalink: clipLine
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">clipLine</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::clipLine(
    Rect imgRect,
    Point& pt1,
    Point& pt2 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool Cv2.ClipLine(
    Rect imgRect,
    ref Point pt1,
    ref Point pt2
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, pt1, pt2 = cv2.clipLine(
    imgRect,
    pt1,
    pt2
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<font color="#c7254e">클리핑(Clipping)</font>이란 특정 직선이 일정 영역 밖으로 나가는 부분을 제외하는 알고리즘입니다. 
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력된 사각형을 가로지르는 직선의 교차점을 계산합니다.

### 매개변수(Parameter)

> `영역(imgRect)` 클리핑을 계산하려는 영역

> `지점 1(pt1)` 직선의 시작

> `지점 2(pt2)` 직선의 끝

### 반환값(Returns)

> `결괏값(retval)` 직선이 영역 안에 있는 경우, 참(True) 값을 반환

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">지점 1(pt1)</a> 영역과 직선의 교차점 1

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">지점 2(pt2)</a> 영역과 직선의 교차점 2