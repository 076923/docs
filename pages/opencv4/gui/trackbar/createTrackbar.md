---
title: 트랙 바 생성
sidebar: opencv4_sidebar
permalink: createTrackbar
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">createTrackbar</h2>
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
<pre class="prettyprint"><code class="language-cpp">int cv::createTrackbar(
    const String& trackbarname,
    const String& winname,
    int* value,
    int count,
    TrackbarCallback onChange = 0,
    void* userdata = 0
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">int Cv2.CreateTrackbar(
    string trackbarName,
    string winName,
    ref int value,
    int count,
    TrackbarCallbackNative onChange = null,
    IntPtr userData = default
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.createTrackbar(
    trackbarName,
    windowName,
    value,
    count,
    onChange
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 이름의 윈도우에 트랙 바를 생성합니다.

### 매개변수(Parameter)

> `트랙 바 이름(trackbarName)` 생성하려는 트랙 바 이름

> `윈도우 이름(winname)` 적용하려는 윈도우 이름

> `초깃값(value)` 트랙 바의 초기 슬라이더 위치

> `최댓값(count)` 트랙 바의 슬라이더 최대 위치

> `콜백 함수(onChange)` 슬라이더의 위치가 변경될 때마다 호출되는 함수

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">사용자 정의 데이터(userdata)</a> 콜백 함수에 함께 전달할 임의의 사용자 데이터

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">결과(retval)</a> 트랙 바를 생성한 경우, 참(1) 값을 반환
