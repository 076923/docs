---
title: 대비 제한 적응형 히스토그램 평활화 클래스 - 타일 크기 속성 반환
sidebar: opencv4_sidebar
permalink: CLAHE-getTilesGridSize
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">CLAHE.getTilesGridSize</h2>
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
<pre class="prettyprint"><code class="language-cpp">Size cv::&lt;CLAHE&gt;::getTilesGridSize()</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Size CLAHE.TilesGridSize</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.CLAHE.getTilesGridSize()</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> `대비 제한 적응형 히스토그램 평활화(Contrast Limited Adaptive Histogram Equalization, CLAHE)` 인스턴스의 `타일 크기(tileGridSize)` 설정값을 반환합니다.

### 매개변수(Parameter)

> `없음`

### 반환값(Returns)

> `타일 크기(retval)` 타일 크기 행과 열의 수