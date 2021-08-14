---
title: 분리형 2D 필터
sidebar: opencv4_sidebar
permalink: sepFilter2D
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">sepFilter2D</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::sepFilter2D(
    Mat src,
    Mat dst,
    int ddepth,
    Mat kernelX,
    Mat kernelY,
    Point anchor = Point(-1,-1),
    double delta = 0,
    int borderType = BORDER_DEFAULT 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.SepFilter2D(
    Mat src,
    Mat dst,
    MatType ddepth,
    Mat kernelX,
    Mat kernelY,
    Point? anchor = null,
    double delta = 0,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.sepFilter2D(
    src,
    ddepth,
    kernelX,
    kernelY,
    anchor = None,
    delta = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<a href="filter2D">2D 필터</a>와 처리 방법이 비슷하지만, 각각의 축에 서로 다른 <font color="#c7254e">커널(Kernel)</font>을 적용할 수 있습니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지에 분리 가능한 임의의 선형 필터를 이미지에 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 임의의 선형 필터를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 임의의 선형 필터가 적용된 이미지

> `출력 이미지 정밀도(ddepth)` 출력 이미지의 정밀도 설정

> `X축 커널(kernelX)` 임의의 선형 필터를 적용하려는 X축 단일 채널 부동 소수점 행렬

> `Y축 커널(kernelX)` 임의의 선형 필터를 적용하려는 Y축 단일 채널 부동 소수점 행렬

> `고정점(anchor)` 필터의 상대적 위치를 나타내는 커널의 중심부

> `오프셋(delta)` 필터링 된 픽셀에 더해지는 값

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 임의의 선형 필터가 적용된 이미지