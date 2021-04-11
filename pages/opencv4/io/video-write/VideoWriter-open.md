---
title: 비디오 쓰기 - 비디오 열기
sidebar: opencv4_sidebar
permalink: VideoWriter-open
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">VideoWriter.open</h2>
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
<pre class="prettyprint"><code class="language-cpp">bool cv::VideoWriter::open(
    const String& filename,
    int apiPreference = CAP_ANY
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">bool VideoWriter.Open(
    string fileName,
    VideoCaptureAPIs apiPreference = VideoCaptureAPIs.ANY
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.VideoWriter.open(
    filename,
    apiPreference
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<b>Linux</b>에서 동영상을 녹화할 때 <font color="#c7254e">FFmpeg</font>를 사용합니다.
{{site.data.alerts.end}}

{{site.data.alerts.note}}
<b>Windows</b>에서 동영상을 녹화할 때 <font color="#c7254e">FFmpeg</font>, <font color="#c7254e">MSWF</font>, <font color="#c7254e">DSHOW</font> 중 하나를 사용합니다.
{{site.data.alerts.end}}

{{site.data.alerts.note}}
<b>MacOSX</b>에서 동영상을 녹화할 때 <font color="#c7254e">AVFoundation</font>를 사용합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
일부 운영체제에서는 <font color="#c7254e">FourCC</font>의 값을 <b>-1</b>로 사용하면 코덱 선택 대화 상자를 띄울 수 있습니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
이미지 시퀸스로 저장하려면 파일 이름을 <b>img_%02d.jpg</b>와 같은 형태로 작성하고, <font color="#c7254e">FourCC</font>와 <font color="#c7254e">fps</font> 값을 <b>0</b>으로 사용합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">FFmpeg</font>가 활성화 된 경우 <font color="#c7254e">FourCC</font> 값을 <b>0</b>으로 사용합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 이미지의 연속을 비디오 파일, 이미지 시퀀스 등으로 작성합니다.

### 매개변수(Parameter)

> `파일 이름(filename)` 비디오 파일의 경로

> [`API 백엔드(apiPreference)`](VideoCaptureAPIs) API 백엔드 식별자

> [`비디오 코덱(fourcc)`](VideoWriter-FourCC) 프레임을 압축하는 데 사용되는 Four Character Code 코드

> `프레임 속도(fps)` 비디오 프레임의 속도

> `프레임 크기(frameSize)` 비디오 프레임의 크기

> `색상 유/무(isColor)` 다중 채널 프레임으로 인코딩 유/무

### 반환값(Returns)

> `생성자(VideoWriter)` VideoWriter 생성자