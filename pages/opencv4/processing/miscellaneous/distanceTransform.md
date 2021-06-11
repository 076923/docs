---
title: 거리 변환
sidebar: opencv4_sidebar
permalink: distanceTransform
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">distanceTransform</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::distanceTransform(
    Mat src,
    Mat dst,
    Mat labels,
    int distanceType,
    int maskSize,
    int labelType = DIST_LABEL_CCOMP
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.DistanceTransform(
    Mat src,
    Mat dst,
    DistanceTypes distanceType,
    DistanceTransformMasks maskSize,
    int dstType = 4
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.distanceTransform(
    src,
    distanceType,
    maskSize,
    dstType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<b>C++의 거리 변환 함수</b>는 <font color="#c7254e">라벨(labels)</font>까지 함께 반환합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">출력 배열 형식(dstType)</font>의 <b>CV_8U</b> 형식은 <font color="#c7254e">거리 계산 방식(distanceType)</font>이 <b>L1</b>일때만 적용할 수 있습니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지의 각 픽셀에 대해 가장 가까운 0 픽셀까지의 거리를 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 거리를 계산하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 배열(dst)</a> 가장 가까운 0 픽셀까지의 거리
 
> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}">라벨(labels)</a> 0 픽셀을 기준으로 라벨링된 라벨 배열

> [`거리 계산 방식(distanceType)`](DistanceTypes) 0 픽셀까지의 거리 계산 방식

> [`거리 변환 마스크 크기(maskSize)`](DistanceTransformMasks) 거리 변환을 위한 마스크 크기

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}" href="DistanceTransformLabelTypes" style="cursor: revert;">거리 변환 라벨링 방식(labelType)</a> 0 픽셀에 가까운 픽셀에 대한 라벨링 방식

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS_Python}}">출력 배열 형식(dstType)</a> 출력 배열의 형식 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 배열(dst)</a> 가장 가까운 0 픽셀까지의 거리