---
title: 아핀 변환
sidebar: opencv4_sidebar
permalink: warpAffine
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">warpAffine</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::warpAffine(
    Mat src,
    Mat dst,
    Mat M,
    Mat dsize,
    int flags = INTER_LINEAR,
    int borderMode = BORDER_CONSTANT,
    const Scalar& borderValue = Scalar() 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.WarpAffine(
    Mat src,
    Mat dst,
    Mat m,
    Size dsize,
    InterpolationFlags flags = InterpolationFlags.Linear,
    BorderTypes borderMode = BorderTypes.Constant,
    Scalar? borderValue = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.warpAffine(
    src,
    M,
    dsize,
    flags = None,
    borderMode = None,
    borderValue = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="
`아핀 변환 계산식(Affine Transform Formula)`
<br><br>
$$ dst(x, y) = src(ax + by + e,\ cx + dy + f) $$
" type="success" %}

<br>

### 요약(Summary)

> 이미지에 아핀 변환을 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 아핀 변환을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 아핀 변환이 적용된 출력 이미지

> `아핀 변환 행렬(M)` 2×3 아핀 변환 행렬

> `절대 크기(dsize)` 출력 이미지의 크기

> [`내삽 방식(interpolation)`](InterpolationFlags) 이미지 내의 픽셀을 내삽하는데 사용되는 계산 방식

> [`외삽 방식(borderMode)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

> `외삽 색상(borderValue)` 외삽된 픽셀의 색상

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 아핀 변환이 적용된 출력 이미지
