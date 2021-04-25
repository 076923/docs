---
title: 색상 맵 적용
sidebar: opencv4_sidebar
permalink: applyColorMap
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">applyColorMap</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::applyColorMap(
    Mat src,
    Mat dst,
    int colormap
)
<hr>
void cv::applyColorMap(
    Mat src,
    Mat dst,
    Mat userColor
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.ApplyColorMap(
    Mat src,
    Mat dst,
    ColormapTypes colormap
)
<hr>
void Cv2.ApplyColorMap(
    Mat src,
    Mat dst,
    Mat userColor
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.applyColorMap(
    src,
    colormap
)
<hr>
dst = cv2.applyColorMap(
    src,
    userColor
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}
<b>사용자 정의 색상 맵(userColor)</b>을 사용할 경우, <font color="#c7254e">순람표(Lookup table)</font> 구조여야 합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `단일 채널 순람표`는 `CV_8UC1` 형식의 `[256, 1]` 형태를 갖습니다.
  
- `단중 채널 순람표`는 `CV_8UC3` 형식의 `[256, 1, 3]` 형태를 갖습니다.

" type="success" %}

<br>

### 요약(Summary)

> 입력 이미지에 색상 맵을 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 색상 맵을 적용하려는 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 색상 맵이 적용된 이미지

> [`색상 맵(colormap)`](ColormapTypes) 적용하려는 색상 맵

> `사용자 정의 색상 맵(userColor)` 적용하려는 사용자 정의 색상 맵 

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 색상 맵이 적용된 이미지