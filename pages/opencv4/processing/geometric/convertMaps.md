---
title: 맵 변환
sidebar: opencv4_sidebar
permalink: convertMaps
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">convertMaps</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::convertMaps(
    Mat map1,
    Mat map2,
    Mat dstmap1,
    Mat dstmap2,
    int dstmap1type,
    bool nninterpolation = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.ConvertMaps(
    Mat map1,
    Mat map2,
    Mat dstmap1,
    Mat dstmap2,
    MatType dstmap1Type,
    bool nnInterpolation = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dstmap1, dstmap2 = cv2.convertMaps(
    map1,
    map2,
    dstmap1type
    nninterpolation = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- `입력 맵 1(map1)`은 `CV_16SC2` 형식, `CV_32FC1` 형식, `CV_32FC2` 형식을 할당할 수 있습니다.
  
- `입력 맵 2(map2)`은 `CV_16UC1` 형식, `CV_32FC1` 형식을 할당하거나 `비어 있는 행렬(None)`을 입력할 수 있습니다.
  
- `출력 맵 형식(dstmap1Type)`은 `CV_16SC2` 형식, `CV_32FC1` 형식, `CV_32FC2` 형식을 할당할 수 있습니다.

" type="success" %}

<br>

### 요약(Summary)

> 이미지 변환 맵의 형식을 변환합니다.

### 매개변수(Parameter)

> `입력 맵 1(map1)` 형식을 변환하려는 변환 맵 1

> `입력 맵 2(map2)` 형식을 변환하려는 변환 맵 2

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 맵 1(dstmap1)</a> 형식이 변환된 출력 맵 1

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 맵 2(dstmap2)</a> 형식이 변환된 출력 맵 2

> `출력 맵 형식(dstmap1Type)` 출력 맵의 형식

> `보간법 사용 유/무(nninterpolation)` 고정 소수점의 보간 유/무를 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 맵 1(dstmap1)</a> 형식이 변환된 출력 맵 1

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 맵 2(dstmap2)</a> 형식이 변환된 출력 맵 2
