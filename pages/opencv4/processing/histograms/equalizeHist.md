---
title: 히스토그램 평활화
sidebar: opencv4_sidebar
permalink: equalizeHist
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">equalizeHist</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::equalizeHist(
    Mat src
    Mat dst
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.EqualizeHist(
    Mat src,
    Mat dst,
    HistCompMethods method
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.equalizeHist(
    src,
    dst = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{% include callout.html content="

- `입력 이미지(src)`의 히스토그램 **누적 분포 함수(Cumulative Distribution Function, cdf)**를 계산합니다.
  
- $$ dst(x,\ y) = cdf(src(x,\ y)) \times \frac{255}{width \times height} $$
  
- $$ cdf $$에 `순람표(Look Up Table, LUT)`을 적용해 계산합니다.
  
- 히스토그램 평활화는 **밝기(Brightness)**를 정규화하고 **대비(Contrast)**를 높입니다.

" type="warning" %}

<br>

### 요약(Summary)

> 그레이스케일 이미지의 히스토그램을 균일한 분포로 변경합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 히스토그램 평활화를 적용하려는 이미지

> `출력 이미지(dst)` 히스토그램 평활화가 적용된 이미지

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 히스토그램 평활화가 적용된 이미지
