---
title: 영역 채우기
sidebar: opencv4_sidebar
permalink: floodFill
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">floodFill</h2>
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
<pre class="prettyprint"><code class="language-cpp">int cv::floodFill(
    Mat image,
    Mat mask,
    Point seedPoint,
    Scalar newVal,
    Rect* rect = 0,
    Scalar loDiff = Scalar(),
    Scalar upDiff = Scalar(),
    int flags = 4
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">int Cv2.FloodFill(
    Mat image,
    Mat mask,
    Point seedPoint,
    Scalar newVal,
    out Rect rect,
    Scalar? loDiff = null,
    Scalar? upDiff = null,
    FloodFillFlags flags = FloodFillFlags.Link4
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, image, mask, rect = cv2.floodFill(
    image,
    mask,
    seedPoint,
    newVal,
    loDiff = None,
    upDiff = None,
    flags = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
이미지 내 특정 조건에 부합하는 영역만 내부 채우기를 적용합니다.
{{site.data.alerts.end}}

{% include callout.html content="

`영역 채우기 조건`
<br><br>
$$ src(x', y') - \text{loDiff} \leq src(x, y) \leq src(x', y') + \text{upDiff} $$

" type="info" %}

{% include callout.html content="

- 마스크 이미지는 `CV_8UC1` 형식과 입력 이미지 크기보다 **2 픽셀이 더 큰 너비와 높이를 가져아 합니다.**

" type="success" %}

### 요약(Summary)

> 입력 이미지의 시작점에서 특정 조건에 부합하는 픽셀 영역을 특정 색상으로 변경합니다.

### 매개변수(Parameter)

> `입력 이미지(image)` 영역 채우기를 적용하려는 입력 이미지

> `마스크 이미지(mask)` 영역 채우기 연산을 위한 마스크 이미지

> `시작점(seedPoint)` 영역 채우기 기준점

> `영역 채우기 색상(newVal)` 영역에 새롭게 채워질 색상

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">최소 면적 사각형(rect)</a> 채워진 영역을 감싸는 최소 면적 사각형

> `하위 차이 임곗값(loDiff)` 영역 채우기 조건의 하위 차이 임곗값

> `상위 차이 임곗값(upDiff)` 영역 채우기 조건의 상위 차이 임곗값

> [`영역 채우기 방식(flags)`](FloodFillFlags) 영역 채우기 방식

### 반환값(Returns)

> `결괏값(retval)` 영역이 채워진 픽셀의 개수

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">입력 이미지(image)</a> 영역 채우기를 적용한 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">마스크 이미지(mask)</a> 영역 채우기를 적용한 마스크 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">최소 면적 사각형(rect)</a> 채워진 영역을 감싸는 최소 면적 사각형