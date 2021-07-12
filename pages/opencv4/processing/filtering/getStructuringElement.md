---
title: 구조 요소 반환
sidebar: opencv4_sidebar
permalink: getStructuringElement
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getStructuringElement</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat cv::getStructuringElement(
    int shape,
    Size ksize,
    Point anchor = Point(-1,-1)
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.GetStructuringElement(
    MorphShapes shape,
    Size ksize,
    Point anchor
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getStructuringElement(
    shape,
    ksize,
    anchor = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
커널(Kernel)보다 더 복잡한 개념인 <font color="#c7254e">구조 요소(Element)</font>를 생성합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">고정점(anchor)</font>에 <font color="#c7254e">null</font> 값이나 <font color="#c7254e">None</font> 값을 사용하면 고정점의 위치는 <font color="#c7254e">(-1, -1)</font>을 갖게 됩니다.<br>
<li class="alerts_li"><font color="#c7254e">(-1, -1)</font>은 <b>커널의 중심부</b>를 의미합니다.</li>
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 모폴로지 연산을 위해 지정된 모양과 크기의 구조 요소를 생성해 반환합니다.

### 매개변수(Parameter)

> [`모양(shape)`](MorphShapes) 구조 요소의 모양

> `크기(ksize)` 구조 요소의 크기

> `고정점(anchor)` 콘벌루션(convolution) 연산을 적용하려는 지점

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">구조 요소(retval)</a> 특정 형태의 구조 요소