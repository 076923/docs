---
title: 양방향 필터
sidebar: opencv4_sidebar
permalink: bilateralFilter
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">bilateralFilter</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::bilateralFilter(
    Mat src,
    Mat dst,
    int d,
    double sigmaColor,
    double sigmaSpace,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.BilateralFilter(
    Mat src,
    Mat dst,
    int d,
    double sigmaColor,
    double sigmaSpace,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.bilateralFilter(
    src, 
    d,
    sigmaColor,
    sigmaSpace,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<b>가장자리(Edge)</b>를 선명하게 보존하면서 노이즈를 우수하게 제거할 수 있습니다.
{{site.data.alerts.end}}

{{site.data.alerts.important}}
<font color="#c7254e">지름(d)</font>이 클수록 수채화처럼 변형되며, 알고리즘의 처리 속도가 매우 느려집니다.
{{site.data.alerts.end}}

{% include callout.html content="

- 이미지를 실시간으로 처리하는 경우에는 `지름(d)`의 값을 **5**로 사용합니다.
  
- 이미지를 실시간으로 처리하지 않는 경우에는 `지름(d)`의 값을 **9**로 사용합니다.
  
- `지름(d)`을 **-1**로 지정하는 경우에는 `시그마 공간(sigmaSpace)`과 비례하도록 설정됩니다. 

" type="warning" %}

{{site.data.alerts.tip}}
<font color="#c7254e">시그마 색상(sigmaColor)</font>이 클수록 흐림 효과에 포함될 강도의 범위가 넓어집니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">시그마 공간(sigmaSpace)</font>이 클수록 값이 클수록 인접한 픽셀에 영향을 미칩니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지에 양방향 필터를 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 양방향 필터를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 양방향 필터가 적용된 이미지

> `지름(d)` 흐림 효과를 적용할 각 픽셀 영역의 지름

> `시그마 색상(sigmaColor)` 색상 공간(color domain)에서 사용할 가우시안 커널의 너비

> `시그마 공간(sigmaSpace)` 좌표 공간(space domain)에서 사용할 가우시안 커널의 너비

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 양방향 필터가 적용된 이미지