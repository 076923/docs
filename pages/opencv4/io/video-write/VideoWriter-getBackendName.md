---
title: 비디오 쓰기 - 백엔드 API 반환
sidebar: opencv4_sidebar
permalink: VideoWriter-getBackendName
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoWriter.getBackendName</h2>
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
<pre class="prettyprint"><code class="language-cpp">string cv::VideoWriter::getBackendName()</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">string VideoWriter.GetBackendName()</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.VideoWriter.getBackendName()</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
녹화를 할 수 있는 상태여야 합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 비디오 쓰기에 사용된 백엔드 API를 반환합니다. 

### 매개변수(Parameter)

> `없음`

### 반환값(Returns)

> `결과(retval)` 비디오 쓰기의 백엔드 API 이름