---
title: 히스토그램 역투영
sidebar: opencv4_sidebar
permalink: calcBackProjection
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">calcBackProjection</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::calcBackProject(
    const Mat* images,
    int nimages,
    const int* channels,
    Mat hist,
    Mat backProject,
    const float** ranges,
    double scale = 1,
    bool uniform = true
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.CalcBackProject(
    Mat[] images,
    int[] channels,
    Mat hist,
    Mat backProject,
    Rangef[] ranges,
    bool uniform = true
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.calcBackProjection(
    images,
    channels,
    hist,
    ranges,
    scale
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- `채널(channels)`은 히스토그램 차원 수와 일치해야 합니다.
  
- 첫 번째 이미지 채널은 `0`부터 `첫 번째 이미지의 채널 수 - 1`로 할당됩니다.
  
- 두 번째 이미지 채널은 `첫 번째 이미지의 채널 수 - 1`에서 `두 번재 이미지의 채널 수 - 1`로 할당됩니다.

" type="success" %}

<br>

### 요약(Summary)

> 히스토그램 역투영을 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(images)` 히스토그램 역투영을 계산하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}">이미지 수(nimages)</a> 입력 이미지의 개수 

> `채널(channels)` 히스토그램 역투영 계산에 사용하려는 채널 목록

> `히스토그램(hist)` 입력 히스토그램

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(backProject)</a> 입력 이미지의 크기와 깊이가 동일한 단일 채널 역투영 이미지

> `범위(ranges)` 각 차원의 히스토그램 빈(Bin) 배열

> `비율(scale)` 히스토그램 역투영된 픽셀에 곱해지는 값

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">균일성(uniform)</a> 히스토그램 균일 여부 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 입력 이미지의 크기와 깊이가 동일한 단일 채널 역투영 이미지
