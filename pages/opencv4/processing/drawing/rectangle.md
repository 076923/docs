---
title: 사각형 그리기
sidebar: opencv4_sidebar
permalink: rectangle
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">rectangle</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::rectangle(
    Mat img,
    Point pt1,
    Point pt2,
    const Scalar& color,
    int thickness = 1,
    int lineType = LINE_8,
    int shift = 0 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Rectangle(
    Mat img,
    Point pt1,
    Point pt2,
    Scalar color,
    int thickness = 1,
    LineTypes lineType = LineTypes.Link8,
    int shift = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">img = cv2.rectangle(
    img,
    pt1,
    pt2,
    color,
    thickness = None,
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
<font color="#c7254e">두께(thickness)</font>가 음수일 경우, 채워진 사각형으로 그립니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 이미지에 사각형을 그립니다.

### 매개변수(Parameter)

> `이미지(img)` 사각형을 그릴려는 이미지

> `지점1(pt1)` 사각형의 좌측 상단 좌표

> `지점2(pt2)` 사각형의 우측 하단 좌표

> `색상(color)` 사각형의 색상

> `두께(thickness)` 사각형의 두께

> [`선형 타입(lineType)`](LineTypes) 선의 유형 설정

> `비트 시프트(shift)` 소수점 이하의 값이 포함된 실숫값 좌표로 그리기 위한 비트 수

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">이미지(img)</a> 사각형이 그려진 이미지