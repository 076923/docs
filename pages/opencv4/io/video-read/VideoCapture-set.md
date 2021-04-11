---
title: 비디오 읽기 - 속성 설정
sidebar: opencv4_sidebar
permalink: VideoCapture-set
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoCapture.set</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::VideoCapture::set(
    int propId,
    double value
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool VideoCapture.Set(
    VideoCaptureProperties propertyId,
    double value
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.VideoCapture.set(
    propId,
    value
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 비디오 읽기 속성을 설정합니다. 

### 매개변수(Parameter)

> [`속성 이름(propId)`](VideoCaptureProperties) 변경하려는 속성 이름

> `속성값(value)` 변경하려는 속성 값

### 반환값(Returns)

> `결괏값(retval)` 백엔드에서 지원되는 경우, 참(True) 값을 반환