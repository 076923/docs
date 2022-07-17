---
title: 대비 제한 적응형 히스토그램 평활화 클래스 - 적용
sidebar: opencv4_sidebar
permalink: CLAHE-apply
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">CLAHE.apply</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::&lt;CLAHE&gt;::apply(
    Mat src,
    Mat dst
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Void CLAHE.Apply(
    Mat src,
    Mat dst
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.CLAHE.apply(
    src,
    dst = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- `입력 이미지(src)`는 `CV_8UC1` 형식, `CV_16UC1` 형식만 가능합니다.

" type="warning" %}

<br>

### 요약(Summary)

> `대비 제한 적응형 히스토그램 평활화(Contrast Limited Adaptive Histogram Equalization, CLAHE)`를 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 대비 제한 적응형 히스토그램 평활화를 적용하려는 이미지
 
> `출력 이미지(dst)` 대비 제한 적응형 히스토그램 평활화가 적용된 이미지

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 대비 제한 적응형 히스토그램 평활화가 적용된 이미지