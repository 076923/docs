---
title: 윈도우 직사각형 크기 반환
sidebar: opencv4_sidebar
permalink: getWindowImageRect
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getWindowImageRect</h2>
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
<pre class="prettyprint"><code class="language-cpp">Rect cv::getWindowImageRect(
    const String& winname
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Rect Cv2.GetWindowImageRect(
    string winName
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getWindowImageRect(
    winname
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 윈도우의 클라이언트 화면의 좌표 및 크기를 반환합니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 직사각형 크기를 확인하려는 윈도우 이름

### 반환값(Returns)

> `직사각형 정보(retval)` 클라이언트 화면의 정보(x 좌표, y 좌표, 너비, 높이)를 반환
