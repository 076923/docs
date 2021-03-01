---
title: 이미지 부호화 검사
sidebar: opencv4_sidebar
permalink: haveImageWriter
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">haveImageWriter</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::haveImageWriter(
    string& filename
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool Cv2.HaveImageWriter(
    string fileName
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.haveImageWriter(
    filename
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> OpenCV에서 특정 파일을 저장할 수 있는지 검사합니다.

### 매개변수(Parameter)

> `파일 이름(filename)` 이미지 파일의 경로


### 반환값(Returns)

> `결과(retval)` 이미지 파일을 OpenCV로 부호화(Encoding)할 수 있는 경우, 참(True) 값을 반환