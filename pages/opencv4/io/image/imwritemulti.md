---
title: 다중 페이지 이미지 쓰기
sidebar: opencv4_sidebar
permalink: imwritemulti
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">imwritemulti</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::imwritemulti(
    const String& filename,
    Mat img,
    const std::vector&lt;int&gt;& params = std::vector&lt;int&gt;() 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool Cv2.ImWrite(
    string fileName,
    Mat img,
    params ImageEncodingParam[] prms
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.imwritemulti(
    filename,
    flags,
    params = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
OpenCvSharp4에서는 지원되지 않습니다. ImWrite를 사용합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.TIFF}}">다중 이미지</a>를 파일로 저장합니다.

### 매개변수(Parameter)

> `파일 이름(filename)` 이미지 파일의 경로

> `이미지(img)` 저장하려는 이미지

> [`이미지 부호화 매개변수(params)`](imageEncodingParam) 부호화 매개변수

### 반환값(Returns)

> `결과(retval)` 파일로 저장할 수 있는 경우, 참(True) 값을 반환