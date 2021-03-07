---
title: 이미지 표시
sidebar: opencv4_sidebar
permalink: imshow
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">imshow</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::imshow(
    const String& winname,
    Mat mat
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.ImShow(
    string winname,
    Mat mat
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">None = cv2.imshow(
    winname,
    mat
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.important}}
<a href="waitKey">키 입력 대기 함수</a>와 함께 사용하지 않을 경우, 이미지가 표시되지 않습니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
이미지 표시 함수는 <b>8 비트 단일 채널</b> 또는 <b>3 채널</b> 이미지에 적합한 함수입니다. 일부 형식은 범위가 변경되어 표시됩니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `CV_8U` 형식 이미지는 변경없이 그대로 표시됩니다.
  
- `CV_16U` 또는 `CV_32S` 형식 이미지는 **256**으로 나눈 값으로 표시됩니다. 즉, [0, 255]의 값으로 매핑됩니다.
  
- `CV_32F` 또는 `CV_64F` 형식 이미지는 **256**으로 곱한 값으로 표시됩니다. 즉, [0, 255]의 값으로 매핑됩니다.

" type="success" %}

<br>

### 요약(Summary)

> 특정 이름의 윈도우에 이미지를 표시합니다. 특정 이름의 윈도우가 없다면, 윈도우를 생성합니다.

### 매개변수(Parameter)

> `윈도우 이름(winname)` 이미지를 표시하려는 윈도우 이름

> `이미지(mat)` 표시하려는 이미지

### 반환값(Returns)

> `없음`
