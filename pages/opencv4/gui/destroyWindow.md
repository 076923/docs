---
title: 윈도우 제거
sidebar: opencv4_sidebar
permalink: destroyWindow
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">destroyWindow</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::destroyWindow(
    const String& winname
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void DestroyWindow(
    string winName
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.destroyWindow(
    winname
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 윈도우를 닫습니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 닫으려는 윈도우 이름

### 반환값(Returns)

> `없음`
