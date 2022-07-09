---
title: 히스토그램 계산
sidebar: opencv4_sidebar
permalink: calcHist
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">calcHist</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::calcHist(
    const Mat* images,
    int nimages,
    const int* channels,
    Mat mask,
    Mat hist,
    int dims,
    const int* histSize,
    const float** ranges,
    bool uniform = true,
    bool accumulate = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.CalcHist(
    Mat[] images,
    int[] channels,
    Mat mask,
    Mat hist,
    int dims,
    int[] histSize,
    Rangef[] ranges,
    bool uniform = true,
    bool accumulate = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">hist = cv2.calcHist(
    images,
    channels,
    mask,
    histSize,
    ranges,
    hist = None
    accumulate = None 
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- `입력 이미지(images)`는 `CV_8U` 형식, `CV_16U` 형식, `CV_32F` 형식을 할당할 수 있습니다.
  
- `채널(channels)`은 히스토그램 차원 수와 일치해야 합니다.
        
- 첫 번째 이미지 채널은 `0`부터 `첫 번째 이미지의 채널 수 - 1`로 할당됩니다.

- 두 번째 이미지 채널은 `첫 번째 이미지의 채널 수 - 1`에서 `두 번재 이미지의 채널 수 - 1`로 할당됩니다.
        
- `마스크(mask)`는 `입력 이미지(images)`와 크기가 동일하며 8비트 형식만 가능합니다.

" type="success" %}

<br>

### 요약(Summary)

> 히스토그램을 계산합니다.

### 매개변수(Parameter)

> `입력 이미지(images)` 히스토그램 역투영을 계산하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}">이미지 수(nimages)</a> 입력 이미지의 개수 

> `마스크(mask)` 히스토그램을 검출하려는 특정 관심 영역

> `채널(channels)` 히스토그램 계산에 사용하려는 채널 목록

> `히스토그램(hist)` 입력 이미지로부터 계산된 히스토그램

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">차원(dims)</a> 입력 이미지로부터 계산된 히스토그램 차원

> `히스토그램 크기(histSize)` 각 차원의 히스토그램 빈(Bin) 개수

> `범위(ranges)` 각 차원의 히스토그램 빈(Bin) 범위

> `비율(scale)` 히스토그램 역투영된 픽셀에 곱해지는 값

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">균일성(uniform)</a> 히스토그램 균일 여부 설정

> `누적(accumulate)` 히스토그램(hist)에 누적합 여부 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">히스토그램(hist)</a> 입력 이미지로부터 계산된 히스토그램
