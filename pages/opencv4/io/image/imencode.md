---
title: 이미지 부호화
sidebar: opencv4_sidebar
permalink: imencode
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
<pre class="prettyprint"><code class="language-cpp">bool cv::imencode(
    String& ext,
    Mat img,
    std::vector&lt;uchar&gt;& buf,
    const std::vector&lt;int&gt;& params = std::vector&lt;int&gt;() 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.ImEncode(
    string ext,
    Mat img,
    out byte[] buf,
    params ImageEncodingParam[] prms
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, buf = cv2.imencode(
    ext,
    img,
    params = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 이미지를 메모리 버퍼로 부호화합니다.

### 매개변수(Parameter)

> [`확장자(ext)`](imageExt) 출력 형식을 정의하는 파일 확장자

> `이미지(img)` 부호화하려는 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">버퍼(buf)*</a> 버퍼로 부호화된 출력 배열

> [`이미지 부호화 매개변수(params)`](imageEncodingParam) 부호화 매개변수

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}">결과(retval)*</a> 이미지 파일을 OpenCV로 부호화(Encoding)할 수 있는 경우, 참(True) 값을 반환

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">버퍼(buf)*</a> 버퍼로 부호화된 출력 배열