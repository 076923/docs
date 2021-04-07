---
title: 비디오 읽기 클래스
sidebar: opencv4_sidebar
permalink: VideoCapture
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoCapture</h2>
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
<pre class="prettyprint"><code class="language-cpp">cv::VideoCapture::VideoCapture(
    const String& filename,
    int apiPreference = CAP_ANY
)
<hr>
cv::VideoCapture::VideoCapture(
    int index,
    int apiPreference = CAP_ANY
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">VideoCapture VideoCapture(
    string fileName,
    VideoCaptureAPIs apiPreference = VideoCaptureAPIs.ANY
)
<hr>
VideoCapture VideoCapture(
    int index,
    VideoCaptureAPIs apiPreference = VideoCaptureAPIs.ANY
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">&lt;VideoCapture object&gt; = cv2.VideoCapture(
    filename,
    apiPreference
)
<hr>
&lt;VideoCapture object&gt; = cv2.VideoCapture(
    index,
    apiPreference
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}
<b>문자열</b>을 입력할 경우, 파일 경로로 간주하여 <font color="#c7254e">동영상 파일</font>을 읽습니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `동영상 파일` : video.avi

" type="success" %} 

{{site.data.alerts.tip}}
<b>문자열 포맷팅(formatting)</b>이 있는 경우, 시퀀스로 간주하여 <font color="#c7254e">다수의 이미지</font>를 읽습니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `이미지 시퀀스` : img_%02d.jpg
  
- `API 백엔드(apiPreference)` 설정 필요
  
" type="success" %} 

{{site.data.alerts.tip}}
<b>URL</b>이 있는 경우, 스트리밍(Streaming)으로 간주하여, <font color="#c7254e">실시간 재생 파일</font>을 읽습니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `URL` : protocol://host:port/script_name?script_params|auth
  
" type="success" %} 

{{site.data.alerts.tip}}
<b>정수</b>를 입력할 경우, 카메라 장치 번호로 간주하여 <font color="#c7254e">카메라</font>를 읽습니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `카메라` : 0

" type="success" %} 

<br>

### 요약(Summary)

> 비디오 파일, 카메라, IP 비디오 스트림, 이미지 시퀀스 등을 읽습니다.

### 매개변수(Parameter)

> `파일 이름(filename)` 이미지 파일의 경로

> `카메라 장치 번호(index)` 카메라 장치 ID 번호

> [`API 백엔드(apiPreference)`](VideoCaptureAPIs) API 백엔드 식별자

### 반환값(Returns)

> `생성자(VideoCapture)` VideoCapture 생성자