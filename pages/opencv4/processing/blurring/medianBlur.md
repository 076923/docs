---
title: 중간값 흐림 효과
sidebar: opencv4_sidebar
permalink: medianBlur
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">medianBlur</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::medianBlur(
    Mat src,
    Mat dst,
    int ksize 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.MedianBlur(
    Mat src,
    Mat dst,
    int ksize
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.medianBlur
    src,
    ksize
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
중간값 필터를 사용하여 이미지를 흐리게합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `입력 이미지(src)`는 `CV_8U` 형식, `CV_16U` 형식, `CV_32F` 형식을 할당할 수 있습니다.
  
- `커널 크기(ksize)`는 3 이상의 홀수여야 합니다.

" type="success" %}

<br>

### 요약(Summary)

> 입력 이미지에 중간값 흐림 효과를 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 중간값 흐림 효과를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 중간값 흐림 효과가 적용된 이미지

> `커널 크기(ksize)` 커널의 크기

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 중간값 흐림 효과가 적용된 이미지