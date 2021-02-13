---
title: 윈도우 생성
sidebar: opencv4_sidebar
permalink: namedWindow
folder: opencv4
datatable: true
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">namedWindow</h2>
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
<pre class="prettyprint"><code class="language-cpp">cv::namedWindow(
    string winname,
    int flags = WINDOW_AUTOSIZE
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Cv2.NamedWindow(
    string winname,
    WindowMode flags = WindowMode.KeepRatio
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">cv2.namedWindow(
    winname,
    flags = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

### 요약(Summary)

> 특정 이름의 윈도우를 생성합니다. 동일한 이름의 윈도우가 존재할 경우, 아무 동작도 하지 않습니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 윈도우 이름 및 제목 표시줄의 이름을 설정합니다.

> `윈도우 모드(flags)` 표시될 윈도우의 속성을 설정합니다.

<h4 class="page-header">윈도우 모드(flags)</h4>

<div class="datatable-begin"></div>

언어     | 플래그             | 설명                                                             |
-------- | ----------------- | ---------------------------------------------------------------- | 
`C++`    | WINDOW_NORMAL | 윈도우 크기를 조절할 수 있으며, 최대화된 창을 이전 크기로 복원 | 
`C#`     | WindowMode.Normal | 윈도우 크기를 조절할 수 있으며, 최대화된 창을 이전 크기로 복원 | 
`Python` | cv2.WINDOW_NORMAL | 윈도우 크기를 조절할 수 있으며, 최대화된 창을 이전 크기로 복원 | 
`C++`    | WINDOW_AUTOSIZE | 윈도우 크기를 조절할 수 없으며, 이미지의 크기와 동일하게 표시 | 
`C#`     | WindowMode.AutoSize | 윈도우 크기를 조절할 수 없으며, 이미지의 크기와 동일하게 표시 | 
`Python` | cv2.WINDOW_AUTOSIZE | 윈도우 크기를 조절할 수 없으며, 이미지의 크기와 동일하게 표시 | 
`C++`    | WINDOW_FULLSCREEN | 윈도우를 최대화 | 
`C#`     | WindowMode.FullScreen | 윈도우를 최대화 | 
`Python` | cv2.WINDOW_FULLSCREEN | 윈도우를 최대화 | 
`C++`    | WINDOW_KEEPRATIO | 이미지 비율을 최대한 유지 | 
`C#`     | WindowMode.KeepRatio | 이미지 비율을 최대한 유지 | 
`Python` | cv2.WINDOW_KEEPRATIO | 이미지 비율을 최대한 유지 | 
`C++`    | WINDOW_FREERATIO | 비율의 제한이 없는 경우 이미지를 최대한 확장 | 
`C#`     | WindowMode.FreeRatio | 비율의 제한이 없는 경우 이미지를 최대한 확장 | 
`Python` | cv2.WINDOW_FREERATIO | 비율의 제한이 없는 경우 이미지를 최대한 확장 | 
`C++`    | WINDOW_OPENGL | OpenGL을 지원하는 윈도우 | 
`C#`     | WindowMode.OpenGL | OpenGL을 지원하는 윈도우 | 
`Python` | cv2.WINDOW_OPENGL | OpenGL을 지원하는 윈도우 | 

<div class="datatable-end"></div>

### 반환값(Returns)

> `없음`
