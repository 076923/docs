---
title: 윈도우 크기 조정
sidebar: opencv4_sidebar
permalink: resizeWindow
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">resizeWindow</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::resizeWindow(
    const String& winname,
    const cv::Size& size
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.ResizeWindow(
    string winName,
    Size size
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.resizeWindow(
    winname,
    size
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 이름의 윈도우의 크기를 조정합니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 크기를 조정하려는 윈도우 이름

> `크기(size)` 변경할 크기

### 반환값(Returns)

> `없음`
