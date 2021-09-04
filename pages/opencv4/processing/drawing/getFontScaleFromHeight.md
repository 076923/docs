---
title: 글꼴 높이 반환
sidebar: opencv4_sidebar
permalink: getFontScaleFromHeight
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getFontScaleFromHeight</h2>
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
<pre class="prettyprint"><code class="language-cpp">double cv::getFontScaleFromHeight(
    const int fontFace,
    const int pixelHeight,
    const int thickness = 1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">double Cv2.GetFontScaleFromHeight(
    HersheyFonts fontFace,
    int pixelHeight,
    int thickness = 1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getFontScaleFromHeight(
    fontFace,
    pixelHeight,
    thickness = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 픽셀 단위 높이가 되는 글꼴의 크기를 계산합니다.

### 매개변수(Parameter)

> [`글꼴(fontFace)`](HersheyFonts) 크기를 계산하려는 글꼴

> `픽셀 단위 높이(pixelHeight)` 크기를 계산하려는 글꼴의 픽셀 높이

> `두께(thickness)` 크기를 계산하려는 글꼴의 두께

### 반환값(Returns)

> `글꼴 크기(retval)` 글꼴의 크기