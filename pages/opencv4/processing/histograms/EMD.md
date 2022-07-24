---
title: EMD(Earth Mover's Distance) 계산
sidebar: opencv4_sidebar
permalink: EMD
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">EMD</h2>
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
<pre class="prettyprint"><code class="language-cpp">float cv::EMD(
    Mat signature1,
    Mat signature2,
    int distType,
    Mat cost = noArray(),
    float* lowerBound = 0,
    OutputArray flow = noArray() 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">float Cv2.EMD(
    Mat signature1,
    Mat signature2,
    DistanceTypes distType,
    Mat cost,
    out float lowerBound,
    OutputArray flow = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval, lowerBound, flow = cv2.EMD(
    signature1,
    signature2,
    distType,
    cost = None,
    lowerBound = None,
    flow = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- `시그니처(signature)`는 `CV_32FC1` 형식을 할당할 수 있습니다.
  
- `시그니처(signature)`는 **[[가중치, 행 번호, 열 번호], [...]]**의 형태를 지닙니다.
        
- **(3, 3)** 크기의 배열을 `시그니처(signature)`로 변환한다면, **(9, 3)**의 크기를 갖습니다.
  
- `시그니처(signature)`의 가중치는 음수가 아니며, 0이 아닌 값이 하나 이상 있어야 합니다.
          
- 두 시그니처 사이의 거리가 `하한(lowerBound)`보다 크거나 같으면 EMD를 계산하지 않습니다.

" type="success" %}

<br>

### 요약(Summary)

> 두 가중치 지점에 대한 최소 작업 거리를 계산합니다.

### 매개변수(Parameter)

> `시그니처1(signature1)` EMD를 계산하려는 원본 시그니처

> `시그니처1(signature1)` EMD를 계산하려는 대상 시그니처

> [`거리 계산 방식(distanceType)`](DistanceTypes) 시그니처 거리 계산 방식

> `비용(cost)` 사용자 정의 비용 행렬

> `하한(lowerBound)` 두 시그니처 사이의 거리 제한값

> `흐름(flow)` 시그니처1이 시그니처2로 변환되기 위한 최적화 이동 값

### 반환값(Returns)

> `결괏값(retval)` 최적화 비용

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">하한(lowerBound)</a> 두 시그니처 사이의 거리 임곗값

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">흐름(flow)</a> 시그니처1이 시그니처2로 변환되기 위한 최적화 이동 값
