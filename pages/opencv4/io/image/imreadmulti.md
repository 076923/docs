---
title: 다중 페이지 이미지 읽기
sidebar: opencv4_sidebar
permalink: imreadmulti
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">imreadmulti</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::imreadmulti(
    const String& filename,
    std::vector&lt;Mat&gt;& mats,
    int flags = IMREAD_ANYCOLOR
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool Cv2.ImReadMulti(
    string filename,
    out Mat[] mats, 
    ImreadModes flags = ImreadModes.AnyColor
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, mats = cv2.imreadmulti(
    filename,
    mats = None,
    flags = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 파일에서 여러 개의 [이미지](imageExt)를 읽습니다.

### 매개변수(Parameter)

> `파일 이름(filename)` 이미지 파일의 경로

> `이미지 배열(mats)` 출력 이미지

> [`이미지 읽기 방식(flag)`](imreadModes) 이미지 변환 방식

### 반환값(Returns)

> `결괏값(retval)` 이미지 파일을 읽은 경우, 참(True) 값을 반환

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">이미지 배열(mats)*</a> 출력 이미지