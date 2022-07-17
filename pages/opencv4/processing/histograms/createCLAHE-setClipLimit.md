---
title: 대비 제한 적응형 히스토그램 평활화 클래스 - 대비 제한 속성 설정
sidebar: opencv4_sidebar
permalink: CLAHE-setClipLimit
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">CLAHE.setClipLimit</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::&lt;CLAHE&gt;::setClipLimit(
    double clipLimit
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">double CLAHE.ClipLimit</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.CLAHE.setClipLimit(
    clipLimit
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> `대비 제한 적응형 히스토그램 평활화(Contrast Limited Adaptive Histogram Equalization, CLAHE)` 인스턴스의 `대비 제한(clipLimit)`을 설정합니다.

### 매개변수(Parameter)

> `대비 제한(retval)` 대비 제한 임곗값

### 반환값(Returns)

> `없음`