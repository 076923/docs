---
title: 윤곽선 그리기
sidebar: opencv4_sidebar
permalink: drawContours
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">drawContours</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::drawContours(
    Mat image,
    Mat contours,
    int contourIdx,
    const Scalar& color,
    int thickness = 1,
    int lineType = LINE_8,
    Mat hierarchy = noArray(),
    int maxLevel = INT_MAX,
    Point offset = Point()
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.DrawContours(
    Mat image,
    IEnumerable&lt;Mat&gt; contours,
    int contourIdx,
    Scalar color,
    int thickness = 1,
    LineTypes lineType = LineTypes.Link8,
    Mat hierarchy = null,
    int maxLevel = int.MaxValue,
    Point? offset = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">image = cv2.drawContours(
    image,
    contours,
    contourIdx,
    color,
    thickness = None,
    lineType = None,
    hierarchy = None,
    maxLevel = None,
    offset = None
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
<font color="#c7254e">윤곽선 색인(contourIdx)</font>가 음수일 경우, 모든 윤곽선을 그립니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">두께(thickness)</font>가 음수일 경우, 채워진 원으로 그립니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 이미지에 윤곽선을 그립니다.

### 매개변수(Parameter)

> `이미지(image)` 윤곽선을 그릴려는 이미지

> `윤곽선(contours)` 그리려는 윤곽선

> `윤곽선 색인(contourIdx)` 그리려는 윤곽선의 색인 번호

> `색상(color)` 윤곽선의 색상

> `두께(thickness)` 윤곽선의 두께

> [`선형 타입(line_type)`](LineTypes) 선의 유형 설정

> `계층 구조(hierarchy)` 윤곽선 검출 함수에서 반횐된 계층 구조

> `계층 구조 최대 레벨(maxLevel)` 그리려는 윤곽선 계층 구조의 최대 깊이

> `오프셋(offset)` 윤곽선 좌푯값에 더해지는 값 


### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">이미지(image)</a> 윤곽선이 그려진 이미지