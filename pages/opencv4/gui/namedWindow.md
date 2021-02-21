---
title: 윈도우 생성
sidebar: opencv4_sidebar
permalink: namedWindow
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">namedWindow</h2>
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
<pre class="prettyprint"><code class="language-cpp">cv::namedWindow(
    string winname,
    int flags = WINDOW_AUTOSIZE
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Cv2.NamedWindow(
    string winname,
    WindowMode flags = WindowMode.KeepRatio
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">cv2.namedWindow(
    winname,
    flags = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 이름의 윈도우를 생성합니다. 동일한 이름의 윈도우가 존재할 경우, 아무 동작도 하지 않습니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 윈도우 이름 및 제목 표시줄의 이름

> [`윈도우 모드(flags)`](windowMode) 표시될 윈도우의 속성

### 반환값(Returns)

> `없음`
