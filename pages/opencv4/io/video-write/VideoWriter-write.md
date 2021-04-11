---
title: 비디오 쓰기 - 프레임 쓰기
sidebar: opencv4_sidebar
permalink: VideoWriter-write
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoWriter.write</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::VideoWriter::write(
    Mat image
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void VideoWriter.Write(
    Mat image
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.VideoWriter.write(
    image
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
비디오에 작성되는 프레임은 BGR 형식의 이미지를 저장합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 비디오 쓰기에서 프레임을 기록합니다.

### 매개변수(Parameter)

> `프레임(image)` 비디오 쓰기에 인코딩되는 프레임

### 반환값(Returns)

> `없음`