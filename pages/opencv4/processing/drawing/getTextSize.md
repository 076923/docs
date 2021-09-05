---
title: 문자열 크기 반환
sidebar: opencv4_sidebar
permalink: getTextSize
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getTextSize</h2>
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
<pre class="prettyprint"><code class="language-cpp">Size cv::getTextSize(
    const String& text,
    int fontFace,
    double fontScale,
    int thickness,
    int* baseLine
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Size Cv2.GetTextSize(
    string text,
    HersheyFonts fontFace,
    double fontScale,
    int thickness,
    out int baseLine
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, baseLine = cv2.getTextSize(
    text,
    fontFace,
    fontScale,
    thickness
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

>  문자열의 너비와 높이를 계산합니다.

### 매개변수(Parameter)

> `문자열(text)` 크기를 계산하려는 문자열

> [`글꼴(fontFace)`](HersheyFonts) 크기를 계산하려는 글꼴

> `글꼴 크기(fontScale)` 크기를 계산하려는 글꼴의 크기

> `두께(thickness)` 크기를 계산하려는 글꼴의 두께

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">기준선(baseLine)</a> 하단 텍스트 포인트를 기준으로 한 Y 좌표

### 반환값(Returns)

> `문자열 크기(retval)` 문자열의 너비 높이

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">기준선(baseLine)</a> 하단 텍스트 포인트를 기준으로 한 Y 좌표