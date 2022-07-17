---
title: 대비 제한 적응형 히스토그램 평활화 클래스
sidebar: opencv4_sidebar
permalink: createCLAHE
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">createCLAHE</h2>
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
<pre class="prettyprint"><code class="language-cpp">Ptr&lt;CLAHE&gt; cv::createCLAHE(
    double clipLimit = 40.0,
    Size tileGridSize = Size(8, 8)
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">CLAHE Cv2.CreateCLAHE(
    double clipLimit = 40.0,
    Size? tileGridSize = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.createCLAHE(
    clipLimit = 40.0,
    tileGridSize = (8, 8)
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- 히스토그램의 *누적 분포 함수(Cumulative Distribution Function, CDF)*가 급격하게 증가하지 않도록 `대비 제한(clipLimit)`을 설정합니다.
  
- `타일 크기(tileGridSize)`마다 히스토그램 평활화를 진행하고, 타일의 가장자리에 *이중 선형 보간법(Bilinear interpolation)*을 적용합니다.

" type="success" %}

<br>

### 요약(Summary)

> `대비 제한 적응형 히스토그램 평활화(Contrast Limited Adaptive Histogram Equalization, CLAHE)` 클래스 인스턴스를 생성합니다.

### 매개변수(Parameter)

> `대비 제한(clipLimit)` 히스토그램 높이 제한
 
> `타일 크기(tileGridSize)` 히스토그램 균일화를 위한 커널 크기

### 반환값(Returns)

> `생성자(dst)` CLAHE 생성자
