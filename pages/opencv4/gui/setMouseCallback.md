---
title: 마우스 콜백 설정
sidebar: opencv4_sidebar
permalink: setMouseCallback
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">setMouseCallback</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::setMouseCallback(
    const String& winname,
    MouseCallback onMouse,
    void* userdata = 0 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.SetMouseCallback(
    string winName,
    MouseCallback onMouse,
    IntPtr userData = default
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.setMouseCallback(
    windowName,
    onMouse,
    param
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 윈도우에 마우스 핸들러를 설정합니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 속성을 변경하려는 윈도우 이름

> [`마우스 콜백(onMouse)`](MouseCallback) 마우스 이벤트 콜백 함수

> `사용자 정의 데이터(userData)` 콜백 함수와 함께 전달될 사용자 정의 데이터

### 반환값(Returns)

> `없음`