---
title: 트랙 바 위치 설정
sidebar: opencv4_sidebar
permalink: setTrackbarPos
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">setTrackbarPos</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::setTrackbarPos(
    const String& trackbarname,
    const String& winname,
    int pos 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.SetTrackbarPos(
    string trackbarName,
    string winName,
    int pos
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.setTrackbarPos(
    trackbarname,
    winname,
    pos
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 이름의 윈도우에 부착된 트랙 바의 위치를 설정합니다.

### 매개변수(Parameter)

> `트랙 바 이름(trackbarname)` 위치를 변경하려는 트랙 바 이름

> `윈도우 이름(winname)` 위치를 변경하려는 윈도우 이름

> `위치(pos)` 트랙 바의 위치

### 반환값(Returns)

> `없음`
