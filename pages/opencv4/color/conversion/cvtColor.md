---
title: 색상 공간 변환
sidebar: opencv4_sidebar
permalink: cvtColor
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">cvtColor</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::cvtColor(
    Mat src,
    Mat dst,
    int code,
    int dstCn = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.CvtColor(
    Mat src,
    Mat dst,
    ColorConversionCodes code,
    int dstCn = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.cvtColor(
    src,
    code,
    dstCn = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}
<b>8 비트</b> 색상 공간으로 변환하는 경우에는 일부 정보가 손실될 수 있습니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `CV_8U` 형식 이미지는 `0 ~ 255`의 범위를 갖습니다.
  
- `CV_16U` 형식 이미지는 `0 ~ 65,535`의 범위를 갖습니다.
  
- `CV_32F` 형식 이미지는 `0.0 ~ 1.0`의 범위를 갖습니다.

" type="success" %}

<br>

### 요약(Summary)

> 입력 이미지의 색상 공간을 변환합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 색상 공간을 변환하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 색상 공간이 변환된 이미지

> [`색상 공간 변환 코드(code)`](ColorConversionCodes) 변환하려는 색상 공간 코드

> `출력 이미지 채널` 출력 이미지가 갖는 채널 수

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 색상 공간이 변환된 이미지