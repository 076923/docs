---
title: 비디오 쓰기 - 코덱
sidebar: opencv4_sidebar
permalink: VideoWriter-fourcc
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoWriter.fourcc</h2>
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
<pre class="prettyprint"><code class="language-cpp">int cv::VideoWriter::fourcc(
    char c1,
    char c2,
    char c3,
    char c4
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">int VideoWriter.FourCC(
    char c1,
    char c2,
    char c3,
    char c4
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv.VideoWriter.fourcc(
    c1,
    c2,
    c3,
    c4
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 비디오 녹화에 사용할 코덱을 설정합니다.

### 매개변수(Parameter)

> [`코드 1(c1)`](FourCC) 첫 번째 문자

> [`코드 2(c2)`](FourCC) 두 번째 문자

> [`코드 3(c3)`](FourCC) 세 번째 문자

> [`코드 4(c4)`](FourCC) 네 번째 문자

### 반환값(Returns)

> `FourCC(retval)` FourCC 코드