---
title: 적응형 이진화
sidebar: opencv4_sidebar
permalink: adaptiveThreshold
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">adaptiveThreshold</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::adaptiveThreshold(
    Mat src,
    Mat dst,
    double maxval,
    int adaptiveMethod,
    int thresholdType,
    int blockSize,
    double C
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.AdaptiveThreshold(
    Mat src,
    Mat dst,
    double maxval,
    AdaptiveThresholdTypes adaptiveMethod,
    ThresholdTypes thresholdType,
    int blockSize,
    double C
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.adaptiveThreshold(
    src,
    maxValue,
    adaptiveMethod,
    thresholdType,
    blockSize,
    C
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
이미지 내 일정 영역마다 개별적으로 계산된 임곗값을 적용합니다.
{{site.data.alerts.end}}

{% include callout.html content="

`이진화(THRESH_BINARY)`
<br><br>
$$ dst(x, y) = \begin{cases} \text{maxValue} & \text{if:} \ src(x, y) > T(x, y) \\ 0 & \text{else: otherwise} \end{cases} $$
<br><br>
`이진화 역상(THRESH_BINARY_INV)`
<br><br>
$$ dst(x, y) = \begin{cases} 0 & \text{if:} \ src(x, y) > T(x, y) \\ \text{maxValue} & \text{else: otherwise} \end{cases} $$ 
<br><br>
$$ T(x, y) = \frac{1}{blockSize^2} \sum_{x_i}^{} \sum_{y_i}^{} I(x+x_i, y+y_i) - C $$

" type="info" %}

<br>

### 요약(Summary)

> 입력 이미지에 개별적으로 계산된 임곗값을 기준으로 두 영역으로 분리하는 연산을 수행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 적응형 이진화 연산을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 적응형 이진화 연산이 적용된 이미지

> [`적응형 이진화 방식(adaptiveMethod)`](AdaptiveThresholdTypes) 적응형 이진화 방식

> [`임곗값 형식(type)`](ThresholdTypes) 적용하려는 이진화 알고리즘

> `블록 크기(blockSize)` 적응형 이진화 연산에 사용되는 블록 크기

> `상수(C)` 적응형 이진화 연산에 사용되는 상수

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 적응형 이진화 연산이 적용된 이미지