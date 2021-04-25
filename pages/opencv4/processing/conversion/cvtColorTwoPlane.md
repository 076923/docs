---
title: 색상 공간 변환 - YUV
sidebar: opencv4_sidebar
permalink: cvtColorTwoPlane
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">cvtColorTwoPlane</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::cvtColorTwoPlane(
    Mat src1,
    Mat src2,
    Mat dst,
    int code
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.CvtColorTwoPlane(
    Mat src1,
    Mat src2,
    Mat dst,
    ColorConversionCodes code
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.cvtColorTwoPlane(
    src1,
    src2,
    code
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}
<b>YUV 공간</b>에서 <b>BGR 공간</b> 또는 <b>RGB 공간</b>으로만 변환이 가능합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `Y 공간`은 8 비트 단일 채널을 갖습니다.
  
- `UV 공간`은 8 비트 다중 채널(2)과 `Y 공간`의 절반의 이미지 크기를 갖습니다.

" type="success" %}

<br>

### 요약(Summary)

> 두 개의 평면으로 저장되는 색상 공간을 하나의 색상 공간으로 변환합니다.

### 매개변수(Parameter)

> `입력 이미지1(src1)` 색상 공간을 변환하려는 Y 공간

> `입력 이미지2(src2)` 색상 공간을 변환하려는 UV 공간

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 색상 공간이 변환된 이미지

> [`색상 공간 변환 코드(code)`](ColorConversionCodes) 변환하려는 색상 공간 코드

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 색상 공간이 변환된 이미지