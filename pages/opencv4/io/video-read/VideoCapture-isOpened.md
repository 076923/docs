---
title: 비디오 읽기 - 성공 여부 확인
sidebar: opencv4_sidebar
permalink: VideoCapture-isOpened
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoCapture.isOpened</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::VideoCapture::isOpened()</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool VideoCapture.IsOpened()</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.VideoCapture.isOpened()</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 비디오 읽기의 성공(초기화) 여부를 확인합니다.

### 매개변수(Parameter)

> `없음`

### 반환값(Returns)

> `결괏값(retval)` 비디오 읽기가 성공(초기화)된 경우, 참(True) 값을 반환