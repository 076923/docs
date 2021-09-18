---
title: 코너의 고윳값과 고유 벡터
sidebar: opencv4_sidebar
permalink: cornerEigenValsAndVecs
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">cornerEigenValsAndVecs</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::cornerEigenValsAndVecs(
    Mat src,
    Mat dst,
    int blockSize,
    int ksize,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.CornerEigenValsAndVecs(
    Mat src,
    Mat dst,
    int blockSize,
    int ksize,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.cornerEigenValsAndVecs(
    src,
    blockSize,
    ksize,
    dst = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
모든 픽셀 p에 대해 블록 크기(blockSize) 이웃 S(p)를 계산합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">입력 이미지(src)</font>는 <b>단일 채널 8 비트</b> 형식 이미지를 사용하거나, <b>부동 소수점</b> 형식 이미지를 사용합니다.<br>
<font color="#c7254e">출력 이미지(dst)</font>는 <font color="#c7254e">CV_32FC6</font> 형식을 반환합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- **공변량 행렬(Covariation matrix)**의 **미분(Derivatives)**은 `소벨(Sobel)` 연산자를 활용합니다.
  
- $$ x_1 $$, $$ y_1 $$은 $$ \lambda _1 $$의 고유 벡터입니다.
  
- $$ x_2 $$, $$ y_2 $$은 $$ \lambda _2 $$의 고유 벡터입니다.
  
- $$ \lambda _1 $$, $$ \lambda _2 $$는 **행렬(M)**의 정렬되지 않은 고윳값입니다.
  
" type="success" %}

<blockquote class="formula">
<b>공변량 행렬 미분 계산식(Covariation matrix of derivatives Formula):</b>
$$ M = \begin{bmatrix} \sum _{S(p)}(\frac{dI}{dx})^2 & \sum _{S(p)}\frac{dI}{dx} \frac{dI}{dy} \\ \sum _{S(p)}\frac{dI}{dx} \frac{dI}{dy} & \sum _{S(p)}(\frac{dI}{dy})^2 \end{bmatrix} $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 코너 검출을 위한 고윳값과 고유 벡터를 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 고윳값과 고유 벡터를 계산하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 고윳값과 고유 벡터가 계산된 이미지

> `블록 크기(blockSize)` 이웃(Neighborhood)의 크기

> `커널 크기(ksize)` 소벨(Sobel) 커널의 크기

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 고윳값과 고유 벡터가 계산된 이미지