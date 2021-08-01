---
title: 모폴로지 연산
sidebar: opencv4_sidebar
permalink: morphologyEx
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">morphologyEx</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::morphologyEx(
    Mat src,
    Mat dst,
    int op,
    Mat kernel,
    Point anchor = Point(-1,-1),
    int iterations = 1,
    int borderType = BORDER_CONSTANT,
    const Scalar& borderValue = morphologyDefaultBorderValue()
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.MorphologyEx(
    Mat src,
    Mat dst,
    MorphTypes op,
    Mat element,
    Point? anchor = null,
    int iterations = 1,
    BorderTypes borderType = BorderTypes.Constant,
    Scalar? borderValue = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.morphologyEx(
    src,
    op,
    kernel,
    anchor = None,
    iterations = None,
    borderType = None,
    borderValue = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<b>팽창(Dilation)</b>과 <b>침식(Erosion)</b>을 활용하여 다양한 형태학적 연산을 진행합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `입력 이미지(src)`는 `CV_8U` 형식, `CV_16U` 형식, `CV_16S` 형식, `CV_32F` 형식, `CV_64F` 형식을 할당할 수 있습니다.
  
- `출력 이미지(dst)`는 `입력 이미지(src)`와 동일한 정밀도를 반환합니다.
  
" type="success" %}

<br>

### 요약(Summary)

> 입력 이미지에 모폴로지 연산을 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 모폴로지 연산을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 모폴로지 연산이 적용된 이미지

> [`모폴로지 연산(op)`](MorphTypes) 모폴로지 연산 유형

> [`커널(kernel)`](getStructuringElement) 모폴로지 연산을 적용하려는 구조 요소

> `고정점(anchor)` 콘벌루션(convolution) 연산을 적용하려는 지점

> `반복 횟수(iterations)` 팽창 연산 반복 횟수

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

> `외삽 색상(borderValue)` 외삽된 픽셀의 색상

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 모폴로지 연산이 적용된 이미지