---
title: 서브 픽셀 반환
sidebar: opencv4_sidebar
permalink: getRectSubPix
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getRectSubPix</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::getRectSubPix(
    Mat image,
    Size patchSize,
    Point2f center,
    Mat patch,
    int patchType = -1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.GetRectSubPix(
    Mat image,
    Size patchSize,
    Point2f center,
    OutputArray patch,
    int patchType = -1
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">patch = cv2.getRectSubPix(
    image,
    patchSize,
    center,
    patchType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
좌표가 정수가 아니라면 <b>이중 선형 보간법(Bilinear interpolation)</b>으로 픽셀값을 계산합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `중심점(center)`은 이미지 내부에 있어야 합니다.
  
- `패치 크기(patchSize)`가 이미지 영역 밖을 포함한다면 해당 픽셀은 이중 선형 보간법을 적용합니다. 
  
- 다중 채널 이미지의 **모든 채널은 독립적으로 픽셀을 계산해 반환합니다.**
  
" type="success" %}

<blockquote class="formula">
<b>패치 계산식(Patch Formula):</b>
$$ \text{patch}(x,\ y) = \text{src}(x + \text{center}.x - (\text{dst.cols} - 1) \times 0.5, \ y + \text{center}.y - (\text{dst.rows} − 1) \times 0.5 ) $$
</blockquote>

<br>

### 요약(Summary)

> 사각형 영역 내부에 있는 서브 픽셀을 반환합니다.

### 매개변수(Parameter)

> `입력 이미지(image)` 서브 픽셀을 계산하려는 입력 이미지

> `패치 크기(patchSize)` 패치의 크기

> `중심점(center)` 패치의 중심점

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">패치(patch)</a> 서브 픽셀이 계산된 이미지

> `패치 출력 정밀도(patchType)` 패치의 출력 정밀도 설정

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">패치(patch)</a> 서브 픽셀이 계산된 이미지