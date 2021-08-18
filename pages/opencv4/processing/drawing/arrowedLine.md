---
title: 화살표 그리기
sidebar: opencv4_sidebar
permalink: arrowedLine
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">arrowedLine</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::arrowedLine(
    Mat img,
    Point pt1,
    Point pt2,
    const Scalar& color,
    int thickness = 1,
    int line_type = 8,
    int shift = 0,
    double tipLength = 0.1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.ArrowedLine(
    Mat img,
    Point pt1,
    Point pt2,
    Scalar color,
    int thickness = 1,
    LineTypes lineType = LineTypes.Link8,
    int shift = 0,
    double tipLength = 0.1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">img = cv2.arrowedLine(
    img,
    pt1,
    pt2,
    color,
    thickness = None,
    line_type = None,
    shift = None,
    tipLength = None
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

> 이미지에 화살표를 그립니다.

### 매개변수(Parameter)

> `이미지(img)` 화살표를 그릴려는 이미지

> `지점 1(pt1)` 화살표의 끝 부분

> `지점 2(pt2)` 화살표의 촉 부분

> `색상(color)` 화살표의 색상

> `두께(thickness)` 화살표읟 두께

> [`선형 타입(line_type)`](LineTypes) 선의 유형 설정

> `비트 시프트(shift)` 소수점 이하의 값이 포함된 실숫값 좌표로 그리기 위한 비트 수

> `화살표 크기(tipLength)` 화살표의 크기

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">이미지(img)</a> 화살표가 그려진 이미지