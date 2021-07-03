---
title: 리매핑
sidebar: opencv4_sidebar
permalink: remap
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">remap</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::remap(
    Mat src,
    Mat dst,
    Mat map1,
    Mat map2,
    int interpolation,
    int borderMode = BORDER_CONSTANT,
    const Scalar& borderValue = Scalar()
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Remap(
    Mat src,
    Mat dst
    Mat map1,
    Mat map2,
    InterpolationFlags interpolation = InterpolationFlags.Linear,
    BorderTypes borderMode = BorderTypes.Constant,
    Scalar? borderValue = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.remap(
    src,
    map1,
    map2,
    interpolation = None,
    borderMode = None,
    borderValue = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

<blockquote class="formula">
<b>리매핑 계산식(Remapping Formula):</b>
$$ \text{dst}(x, y) = \text{src}(map_{x}(x, y), \ map_{y}(x, y)) $$
</blockquote>

<br>

### 요약(Summary)

> 이미지 픽셀들의 좌표를 임의의 특정 좌표로 옮겨 매핑합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 매핑하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 리매핑된 출력 이미지

> `X축 행렬(map1)` X축 좌표 색인 행렬

> `Y축 행렬(map2)` Y축 좌표 색인 행렬

> [`내삽 방식(interpolation)`](InterpolationFlags) 이미지 내의 픽셀을 내삽하는데 사용되는 계산 방식

> [`외삽 방식(borderMode)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

> `외삽 색상(borderValue)` 외삽된 픽셀의 색상

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 리매핑된 출력 이미지
