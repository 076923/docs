---
title: 코너 서브 픽셀
sidebar: opencv4_sidebar
permalink: cornerSubPix
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">cornerSubPix</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::cornerSubPix(
    Mat image,
    Mat corners,
    Size winSize,
    Size zeroZone,
    TermCriteria criteria 
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Point2f[] Cv2.CornerSubPix(
    Mat image,
    IEnumerable&lt;Point2f&gt; inputCorners,
    Size winSize,
    Size zeroZone,
    TermCriteria criteria
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">corners = cv2.cornerSubPix(
    image,
    corners,
    winSize,
    zeroZone,
    criteria
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
중심 q에서 q의 이웃 내에 위치한 점 p까지의 모든 벡터가 이미지와 노이즈에 영향을 받는 p의 <b>이미지의 강도 또는 색상의 방향 변화(Image Gradient)</b>와 직교한다는 관측을 기반으로 결정됩니다.<br>
방정식은 자기 상관 행렬의 역행렬로 풀 수 있는 선형 시스템을 구성됩니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">입력 이미지(src)</font>는 <b>단일 채널 8 비트</b> 형식 이미지를 사용하거나, <b>부동 소수점</b> 형식 이미지를 사용합니다.<br>
<font color="#c7254e">윈도 크기(winSize)</font>는 <font color="#c7254e">(winSize.X × 2 + 1) × (winSize.Y × 2 + 1)</font>의 크기로 계산됩니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>코너 서브 픽셀(Corner Sub Pixel Formula):</b>
$$ \epsilon _i = {DI_{p_i}}^T \cdot (q - p_i) $$
$$ \sum _i(DI_{p_i} \cdot {DI_{p_i}}^T) \cdot q - \sum _i(DI_{p_i} \cdot {DI_{p_i}}^T \cdot p_i) $$
$$ q = G^{-1} \cdot b $$
</blockquote>

<br>

### 요약(Summary)

> 코너의 위치를 미세 조정합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 코너 서브 픽셀을 계산하려는 입력 이미지

> `코너(corners)` 코너의 위치

> `검출 크기(winSize)` 검출하려는 이웃(Neighborhood)의 크기

> `제외 크기(zeroZone)` 검출 영역에서 제외하려는 부분

> [`종료 기준(termcrit)`](TermCriteria) 반복 알고리즘의 종료 기준

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_CS_Python}}">코너(corners)</a> 코너의 위치