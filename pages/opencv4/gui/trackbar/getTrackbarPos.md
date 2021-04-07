---
title: 트랙 바 위치 반환
sidebar: opencv4_sidebar
permalink: getTrackbarPos
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getTrackbarPos</h2>
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
<pre class="prettyprint"><code class="language-cpp">int cv::getTrackbarPos(
    const String& trackbarname,
    const String& winname
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">int Cv2.GetTrackbarPos(
    string trackbarName,
    string winName
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getTrackbarPos(
    trackbarname,
    winname
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 이름의 윈도우에 부착된 트랙 바의 값을 반환합니다.

### 매개변수(Parameter)

> `트랙 바 이름(trackbarname)` 확인하려는 트랙 바 이름

> `윈도우 이름(winname)` 확인하려는 윈도우 이름

### 반환값(Returns)

> `트랙 바 위칫값(retval)` 현재 트랙 바의 위치
