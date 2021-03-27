---
title: 마우스 콜백
sidebar: opencv4_sidebar
permalink: MouseCallback
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">MouseCallback</h2>
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
<pre class="prettyprint"><code class="language-cpp">typedef void(* cv::MouseCallback)(
    int event,
    int x,
    int y,
    int flags,
    void *userdata
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">public delegate void MouseCallback(
    MouseEventTypes @event,
    int x,
    int y,
    MouseEventFlags flags,
    IntPtr userData
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">func(
    event,
    x,
    y,
    flags,
    userdata
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 마우스 콜백 함수를 정의합니다.

### 매개변수(Parameter)

> [`마우스 이벤트(event)`](MouseEventTypes) 입력된 마우스 이벤트

> `x 좌표(x)` 입력된 마우스 x 좌표

> `y 좌표(y)` 입력된 마우스 y 좌표

> [`마우스 플래그(flags)`](MouseEventTypes) 입력된 마우스 플래그

> [`사용자 정의 데이터(userData)`](setMouseCallback) 전달된 사용자 정의 데이터

### 반환값(Returns)

> `없음`