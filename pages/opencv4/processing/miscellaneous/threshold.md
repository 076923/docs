---
title: 이진화
sidebar: opencv4_sidebar
permalink: threshold
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">threshold</h2>
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
<pre class="prettyprint"><code class="language-cpp">double cv::threshold(
    Mat src,
    Mat dst,
    double thresh,
    double maxval,
    int type
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">double Cv2.Threshold(
    Mat src,
    Mat dst,
    double thresh,
    double maxval,
    ThresholdTypes type
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, dst = cv2.threshold(
    src,
    thresh,
    maxval
    type
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}
<b>오츠 알고리즘(Otsu Algorithm)</b> 또는 <b>삼각형 알고리즘(Triangle Algorithm)</b>은 입력된 임곗값을 사용하지 않고 최적의 임곗값을 계산해 대신 사용합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `오츠 알고리즘(Otsu Algorithm)`과 `삼각형 알고리즘(Triangle Algorithm)`은 **8 비트 단일 채널 이미지**에만 적용할 수 있습니다.

" type="success" %}

<br>

### 요약(Summary)

> 입력 이미지에 임곗값을 기준으로 두 영역으로 분리하는 연산을 수행합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 이진화 연산을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 이진화 연산이 적용된 이미지

> `임곗값(thresh)` 이진화 기준값

> `최댓값(maxval)` 임곗값을 초과했을 때 부여될 값

> [`임곗값 형식(type)`](ThresholdTypes) 적용하려는 이진화 알고리즘

### 반환값(Returns)

> `설정 임곗값(retval)` 이진화 연산에 사용된 임곗값

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 이진화 연산이 적용된 이미지