---
title: 이미지 읽기
sidebar: opencv4_sidebar
permalink: imread
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">imread</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat cv::imread(
    const String& filename,
    int flags = IMREAD_COLOR
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.ImRead(
    string fileName,
    ImreadModes flags = ImreadModes.Color
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.imread(
    filename,
    flags = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 파일에서 [이미지](imageExt)를 읽습니다.

### 매개변수(Parameter)

> `파일 이름(filename)` 이미지 파일의 경로

> [`이미지 읽기 방식(flag)`](imreadModes) 이미지 변환 방식

### 반환값(Returns)

> `출력 이미지(retval)` 출력 이미지