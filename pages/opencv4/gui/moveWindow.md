---
title: 윈도우 이동
sidebar: opencv4_sidebar
permalink: moveWindow
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">moveWindow</h2>
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
<pre class="prettyprint"><code class="language-cpp">cv::moveWindow(
    string winname,
    int x,
    int y
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Cv2.MoveWindow(
    string winname,
    int x,
    int y
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">cv2.moveWindow(
    winname,
    x,
    y
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 이름의 윈도우를 지정된 위치(x, y)로 이동합니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 이동하려는 윈도우 이름을 할당합니다.

> `x 좌표(x)` 이동하려는 윈도우의 x 좌표입니다.

> `y 좌표(y)` 이동하려는 윈도우의 y 좌표입니다.

### 반환값(Returns)

> `없음`
