---
title: 문자열 그리기
sidebar: opencv4_sidebar
permalink: putText
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">putText</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::putText(
    Mat img,
    const String& text,
    Point org,
    int fontFace,
    double fontScale,
    Scalar color,
    int thickness = 1,
    int lineType = LINE_8,
    bool bottomLeftOrigin = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.PutText(
    Mat img,
    string text,
    Point org,
    HersheyFonts fontFace,
    double fontScale,
    Scalar color,
    int thickness = 1,
    LineTypes lineType = LineTypes.Link8,
    bool bottomLeftOrigin = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">img = cv2.putText(
    img,
    text, 
    org,
    fontFace,
    fontScale,
    color,
    thickness = None,
    lineType = None,
    bottomLeftOrigin = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
입력 이미지에 그리기 함수를 직접 적용해 입력 이미지 자체가 변경됩니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 이미지에 문자열을 그립니다.

### 매개변수(Parameter)

> `이미지(img)` 문자열을 그릴려는 이미지

> `문자열(text)` 그리려는 문자열

> `위치(org)` 문자열의 좌측 하단 위치

> [`글꼴(fontFace)`](HersheyFonts) 문자열의 글꼴

> `글꼴 크기(fontScale)` 글꼴의 배율

> `두께(thickness)` 글꼴의 두께

> [`선형 타입(lineType)`](LineTypes) 선의 유형 설정

> `기준점(bottomLeftOrigin)` 거짓(False) 값일 경우, 문자열 그리기 기준을 좌측 상단으로 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">이미지(img)</a> 문자열이 그려진 이미지