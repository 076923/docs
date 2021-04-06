---
title: 비디오 속성 반환
sidebar: opencv4_sidebar
permalink: VideoCapture-get
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoCapture.get</h2>
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
<pre class="prettyprint"><code class="language-cpp">virtual double cv::VideoCapture::get(
    int propId
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">double VideoCapture.Get(
    VideoCaptureProperties propertyId
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.VideoCapture.get(
    propId
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 비디오의 속성을 반환합니다. 

### 매개변수(Parameter)

> [`속성 이름(propId)`](VideoCaptureProperties) 확인하려는 속성 이름

### 반환값(Returns)

> `결과(retval)` 속성에 할당된 결괏값