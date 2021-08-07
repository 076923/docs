---
title: 피라미드 업
sidebar: opencv4_sidebar
permalink: pyrUp
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">pyrUp</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::pyrUp(
    Mat src,
    Mat dst,
    const Size& dstsize = Size(),
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.PyrUp(
    Mat src,
    Mat dst,
    Size? dstSize = null,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.pyrUp(
    src,
    dstsize = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<font color="#c7254e">이미지 피라미드(Image Pyramid)</font>를 활용해 <b>업 샘플링(Up Sampling)</b>하여 하위 단계의 이미지를 생성합니다.
{{site.data.alerts.end}}

{{site.data.alerts.important}}
입력 이미지에 새로운 행과 열을 추가해서 짝수 행과 짝수 열을 만들고 0의 값을 할당합니다. 이후 색상이 결정되지 않는 픽셀은 근삿값으로 채워 가우시안 필터로 컨벌루션을 진행합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>출력 이미지 크기 조건(dstsize Condition):</b>
$$ |\ \text{dstsize.width} - \text{src.cols} \times 2\ | \leq (\text{dstsize.width}\ \text{mod}\ 2) $$
$$ |\ \text{dstsize.height} - \text{src.rows} \times 2\ | \leq (\text{dstsize.height}\ \text{mod}\ 2) $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 업 샘플링 적용하고 흐림 효과를 진행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 업 샘플링을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 업 샘플링이 적용된 이미지

> `출력 이미지 크기(dstsize)` 출력 이미지의 크기

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 업 샘플링이 적용된 이미지