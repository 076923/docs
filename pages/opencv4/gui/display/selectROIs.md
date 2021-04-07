---
title: 다중 관심 영역 선택
sidebar: opencv4_sidebar
permalink: selectROIs
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">selectROIs</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::selectROIs(
    const String& winname,
    Mat img,
    std::vector&lt;Rect&gt;& boundingBoxes,
    bool showCrosshair = true,
    bool fromCenter = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Rect[] Cv2.SelectROIs(
    string windowName,
    Mat img,
    bool showCrosshair = true,
    bool fromCenter = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">boundingBoxes = cv2.selectROIs(
    windowName,
    img,
    showCrosshair = True,
    fromCenter = False
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.tip}}

윈도우에서 왼쪽 마우스 버튼을 누른 상태로 드래그하여 여러 개의 관심 영역을 설정할 수 있습니다. 

{{site.data.alerts.end}}

{% include callout.html content="

- 관심 영역을 설정한 다음 `Space` 키나 `Enter` 키를 눌러 영역을 확정할 수 있습니다.
  
- `C` 키를 눌러 선택 과정을 취소할 수 있습니다.
  
- `ESC` 키를 눌러 관심 영역 설정을 종료할 수 있습니다.

" type="success" %}

<br>

### 요약(Summary)

> 특정 이름의 윈도우에 여러 개의 관심 영역을 선택합니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 관심 영역을 표시하려는 윈도우 이름

> `이미지(img)` 관심 영역을 표시하려는 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}">관심 영역 배열(boundingBoxes)</a> 여러 관심 영역(x 좌표, y 좌표, 너비, 높이)이 저장된 배열

> `십자선 표시(showCrosshair)` 십자선 표시 유/무

> `중심 확장(fromCenter)` 관심 영역이 중심으로부터 확장 유/무

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS_Python}}">관심 영역 배열(boundingBoxes)</a> 여러 관심 영역(x 좌표, y 좌표, 너비, 높이)이 저장된 배열을 반환
