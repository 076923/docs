---
title: 디모자이킹
sidebar: opencv4_sidebar
permalink: demosaicing
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">demosaicing</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::demosaicing(
    Mat src,
    Mat dst,
    int code,
    int dstCn = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Demosaicing(
    Mat src,
    Mat dst,
    ColorConversionCodes code,
    int dstCn = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.demosaicing(
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
`쌍 선형 보간`, `가장자리 인식 보간` `그라디언트 보간` 등으로 디모자이킹을 진행합니다.
{{site.data.alerts.end}}

### 요약(Summary)

> 입력 이미지에 디모자이킹을 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 디모자이킹을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 디모자이킹이 적용된 이미지

> [`색상 공간 변환 코드(code)`](ColorConversionCodes) 변환하려는 색상 공간 코드

> `출력 이미지 채널` 출력 이미지가 갖는 채널 수

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 디모자이킹이 적용된 이미지