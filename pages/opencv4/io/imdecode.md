---
title: 이미지 복호화
sidebar: opencv4_sidebar
permalink: imdecode
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">imdecode</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat dst = cv::imdecode(
    Mat buf,
    int flags
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat dst = Cv2.ImDecode(
    Mat buf,
    ImreadModes flags
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.imdecode(
    buf
    flags
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 메모리에 지정된 버퍼에서 데이터를 복호화해 이미지를 읽습니다.

### 매개변수(Parameter)

> `버퍼(buf)` 이미지로 복호화하려는 바이트 벡터의 입력 배열

> [`이미지 읽기 모드(flag)`](imreadModes) 이미지 변환 방식

### 반환값(Returns)

> `출력 이미지(dst)` 복호화된 결과 이미지