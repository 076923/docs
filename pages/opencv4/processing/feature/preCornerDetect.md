---
title: 코너 특징 맵 검출
sidebar: opencv4_sidebar
permalink: preCornerDetect
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">preCornerDetect</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::preCornerDetect(
    Mat src,
    Mat dst,
    int ksize,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.PreCornerDetect(
    Mat src,
    Mat dst,
    int ksize,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.preCornerDetect(
    src,
    ksize,
    dst = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}
<font color="#c7254e">입력 이미지(src)</font>는 <b>단일 채널 8 비트</b> 형식 이미지를 사용합니다.<br>
<font color="#c7254e">출력 이미지(dst)</font>는 <font color="#c7254e">CV_32F</font> 형식을 반환합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- $$ D_x $$, $$ D_y $$는 이미지의 `일계 도함수(First Derivatives)`를 의미합니다.
  
- $$ D_{xx} $$, $$ D_{yy} $$는 이미지의 `이계 도함수(Second Derivatives)`를 의미합니다.
  
- $$ D_{xy} $$는 이미지의 `혼합 편미분(Mixed Derivatives)`를 의미합니다.

" type="success" %}

<blockquote class="formula">
<b>사전 코너 검출 계산식(Pre Corner Detect Formula):</b>
$$ \text{dst} = (D_x \times \text{src} )^2 \cdot D_{yy} \times \text{src} + (D_y \times \text{src} )^2 \cdot D_{xx} \times  \text{src} - 2 \times D_x \times \text{src} \cdot D_y \times \text{src} \cdot D_{xy} \times \text{src} $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 코너 특징 맵(Feature map)을 검출합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 코너의 특징 맵을 계산하려는 입력 이미지

> `출력 이미지(dst)` 검출된 코너의 특징 맵

> `커널 크기(ksize)` 소벨(Sobel) 커널의 크기

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 검출된 코너의 특징 맵