---
title: 비디오 읽기 - 프레임 반환
sidebar: opencv4_sidebar
permalink: VideoCapture-read
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoCapture.read</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::VideoCapture::read(
    Mat image
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool VideoCapture.Read(
    Mat image
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, image = cv2.VideoCapture.read()</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
비디오에 프레임이 없다면 비어 있는 이미지를 반환합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 비디오 읽기에서 프레임을 읽어 반환합니다.

### 매개변수(Parameter)

> `프레임(image)` 비디오 읽기에서 디코딩된 프레임

### 반환값(Returns)

> `결과(retval)` 프레임을 읽은 경우, 참(True) 값을 반환