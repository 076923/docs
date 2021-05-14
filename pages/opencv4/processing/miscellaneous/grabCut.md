---
title: 그랩 컷
sidebar: opencv4_sidebar
permalink: grabCut
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">grabCut</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::grabCut(
    Mat img,
    Mat mask,
    Rect rect,
    Mat bgdModel,
    Mat fgdModel,
    int iterCount,
    int mode = GC_EVAL
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.GrabCut(
    Mat img,
    Mat mask,
    Rect rect,
    Mat bgdModel,
    Mat fgdModel,
    int iterCount,
    GrabCutModes mode
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">mask, bgdModel, fgdModel = cv2.floodFill(
    img,
    mask,
    rect,
    bgdModel,
    fgdModel,
    iterCount,
    mode
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}

이미지 내 전경과 배경을 찾아 네 가지 그룹으로 나눈 마스크를 반환합니다.

{{site.data.alerts.end}}

{% include callout.html content="

- `확실한 배경 픽셀(GC_BGD)` : 0
  
- `확실한 전경 픽셀(GC_FGD)` : 1
  
- `가능한 배경 픽셀(GC_PR_BGD)` : 2
  
- `가능한 전경 픽셀(GC_PR_FGD)` : 3

" type="info" %}

{% include callout.html content="

`관심 영역(rect)`은 `그랩 컷 방식(mode)`이 **GC_INIT_WITH_RECT**일 때만 사용됩니다. 

" type="success" %}

{% include callout.html content="

- `배경 모델(bgdModel)`과 `전경 모델(fgdModel)`은 **CV_64FC1** 형식의 **[1, 65]** 크기만 가능합니다. 수식은 다음과 같습니다.
  
- `modelSize` = mean + covariance + component weight = 3 + 9 + 1 = **13**
  
- `componentsCount` = **5**
  
- model.cols = `modelSize` * `componentsCount` = **65**

" type="success" %}

<br>

### 요약(Summary)

> 이미지를 전경과 배경으로 분할하는 최적의 컷을 찾습니다.

### 매개변수(Parameter)

> `입력 이미지(img)` 그랩 컷을 적용하려는 입력 이미지

> `마스크 이미지(mask)` 네 가지 그룹으로 분할된 마스크 이미지

> `관심 영역(rect)` 전경이 포함된 관심 영역

> `배경 모델(bgdModel)` 배경 추출을 위한 모델 행렬

> `전경 모델(fgdModel)` 전경 추출을 위한 모델 행렬

> `반복 횟수(iterCount)` 알고리즘 반복 횟수

> [`그랩 컷 방식(mode)`](GrabCutModes) 전경과 배경을 분리할 그랩 컷 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">마스크 이미지(mask)</a> 네 가지 그룹으로 분할된 마스크 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">배경 모델(bgdModel)</a> 배경 추출을 위한 모델 행렬

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">전경 모델(fgdModel)</a> 전경 추출을 위한 모델 행렬