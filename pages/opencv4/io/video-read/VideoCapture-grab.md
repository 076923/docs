---
title: 비디오 읽기 - 그랩
sidebar: opencv4_sidebar
permalink: VideoCapture-grab
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoCapture.grab</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::VideoCapture::grab()</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool VideoCapture.Grab()</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.VideoCapture.grab()</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
카메라가 하드웨어 동기화를 하지 않는 경우에 사용하거나 멀티 헤드 카메라를 사용할 때 적용합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
여러 카메라가 프레임을 동시에 읽는 경우 시간 동기화 오류가 발생합니다.<br>
이를 방지하고자 압축된 형식으로 프레임을 저장해서 여러 카메라가 동시에 동작해도 동기화되어 프레임을 얻을 수 있습니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 비디오에서 프레임을 읽어 내부 버퍼에 저장합니다.

### 매개변수(Parameter)

> `없음`

### 반환값(Returns)

> `결괏값(retval)` 비디오에서 프레임을 가져올 수 있는 경우, 참(True) 값을 반환