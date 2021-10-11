---
title: 코너 검출
sidebar: opencv4_sidebar
permalink: goodFeaturesToTrack
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">goodFeaturesToTrack</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::goodFeaturesToTrack(
    Mat image,
    Mat corners,
    int maxCorners,
    double qualityLevel,
    double minDistance,
    InputArray mask = noArray(),
    int blockSize = 3,
    bool useHarrisDetector = false,
    double k = 0.04 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Point2f[] Cv2.GoodFeaturesToTrack(
    Mat src,
    int maxCorners,
    double qualityLevel,
    double minDistance,
    InputArray mask,
    int blockSize,
    bool useHarrisDetector,
    double k
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">corners = cv2.goodFeaturesToTrack(
    image,
    maxCorners,
    qualityLevel,
    minDistance,
    corners = None,
    mask = None,
    blockSize = None,
    useHarrisDetector = None,
    k = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
입력 이미지에서 <font color="#c7254e">트래킹(Tracking)</font> 하기 좋은 <font color="#c7254e">특징(Feature)</font>를 검출합니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">코너의 최소 고윳값(cornerMinEigenVal)</font> 또는 <font color="#c7254e">해리스 코너 검출(cornerHarris)</font>를 활용해 코너를 검출합니다.
{{site.data.alerts.end}}

<br>

### 요약(Summary)

> 입력 이미지에서 코너를 검출합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 코너를 검출하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}">코너(corners)</a> 코너의 위치

> `코너 최댓값(maxCorners)` 검출할 최대 코너의 수

> `코너 품질(qualityLevel)` 검출된 코너의 최소 품질

> `최소 거리(minDistance)` 검출된 코너들 간의 최소 근접 거리

> `마스크(mask)` 코너를 검출하려는 특정 관심 영역

> `블록 크기(blockSize)` 검출하려는 이웃(Neighborhood)의 크기

> `해리스 코너 검출기(useHarrisDetector)` 해리스 코너 검출 사용 유/무

> `해리스 측정 계수(k)` 해리스 코너 특성 계산식의 k 계수

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS}}">코너(corners)</a> 코너의 위치