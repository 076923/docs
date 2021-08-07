---
title: 피라미드 다운
sidebar: opencv4_sidebar
permalink: pyrDown
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">pyrDown</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::pyrDown(
    Mat src,
    Mat dst,
    const Size& dstsize = Size(),
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.PyrDown(
    Mat src,
    Mat dst,
    Size? dstSize = null,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.pyrDown(
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
<font color="#c7254e">이미지 피라미드(Image Pyramid)</font>를 활용해 <b>다운 샘플링(Down Sampling)</b>하여 상위 단계의 이미지를 생성합니다.
{{site.data.alerts.end}}

{{site.data.alerts.important}}
홀수 크기의 이미지에는 <b>+1</b>을 해서 짝수 크기의 이미지로 변경합니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>출력 이미지 크기 조건(dstsize Condition):</b>
$$ |\ \text{dstsize.width} \times 2 - \text{src.cols}\ | \leq 2 $$
$$ |\ \text{dstsize.height} \times 2 - \text{src.rows}\ | \leq 2 $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 흐림 효과를 적용하고 다운 샘플링을 진행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 다운 샘플링을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 다운 샘플링이 적용된 이미지

> `출력 이미지 크기(dstsize)` 출력 이미지의 크기

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 다운 샘플링이 적용된 이미지