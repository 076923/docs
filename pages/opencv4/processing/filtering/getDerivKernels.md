---
title: 미분 커널 반환
sidebar: opencv4_sidebar
permalink: getDerivKernels
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getDerivKernels</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat cv::getDerivKernels(
    Mat kx,
    Mat ky,
    int dx,
    int dy,
    int ksize,
    bool normalize = false,
    int ktype = CV_32F 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.GetDerivKernels(
    Mat kx,
    Mat ky,
    int dx,
    int dy,
    int ksize,
    bool normalize = false,
    MatType? ktype = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">kx, ky = cv2.getDerivKernels(
    dx,
    dy,
    ksize
    normalize = None,
    ktype = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<font color="#c7254e">크기(ksize)</font>는 <b>-1, 1, 3, 5, 7</b>만 사용할 수 있습니다.<br>
<li class="alerts_li"><font color="#c7254e">-1</font>은 샤르 필터(Scharr filter)를 의미합니다.</li>
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
8 비트 이미지의 정확한 미분 계산하려면 <font color="#c7254e">정규화(normalize)</font>를 <b>거짓(False)</b> 값으로 사용합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `필터 출력 정밀도(ktype)`는 `CV_32F` 형식, `CV_64F` 형식만 가능합니다.

" type="warning" %}

<br>

### 요약(Summary)

> 이미지에서 미분(derivatives)을 계산하기 위한 필터 계수를 반환합니다.

### 매개변수(Parameter)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">행 필터 계수(kx)</a> 행 필터 계수의 출력 행렬

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">열 필터 계수(ky)</a> 열 필터 계수의 출력 행렬

> `X 미분 차수(dx)` X에 대한 미분 차수

> `Y 미분 차수(dy)` Y에 대한 미분 차수

> `크기(ksize)` 필터(커널)의 크기

> `정규화(normalize)` 필터 계수 정규화 유/무

> `필터 출력 정밀도(ktype)` 필터 계수의 출력 정밀도 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">행 필터 계수(kx)</a> 행 필터 계수의 출력 행렬

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">열 필터 계수(ky)</a> 열 필터 계수의 출력 행렬