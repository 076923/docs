---
title: 캐니
sidebar: opencv4_sidebar
permalink: Canny
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">Canny</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::Canny(
    Mat image,
    Mat edges,
    double threshold1,
    double threshold2,
    int apertureSize = 3,
    bool L2gradient = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Canny(
    Mat src,
    Mat edges,
    double threshold1,
    double threshold2,
    int apertureSize = 3,
    bool L2gradient = false
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">edges = cv2.Canny(
    image,
    threshold1,
    threshold2
    apertureSize = None,
    L2gradient = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
<font color="#c7254e">캐니(Canny)</font>는 라플라스 필터 방식을 캐니(J. Canny)가 개선한 방식으로 <b>강한 가장자리</b>를 검출하는 데 목적을 둔 알고리즘입니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
<font color="#c7254e">캐니(Canny)</font> 알고리즘의 동작 순서는 다음과 같습니다.
{{site.data.alerts.end}}

{% include callout.html content="

1. 노이즈 제거를 위해 가우시안 필터를 사용해 흐림 효과를 적용합니다.
  
2. <b>기울기(Gradient)</b> 값이 높은 지점을 검출합니다.(소벨 마스크 적용)
  
3. 최댓값이 아닌 픽셀의 값을 0으로 변경합니다.(명백하게 가장자리가 아닌 값을 제거)
  
4. <b>히스테리시스 임곗값(hysteresis threshold)</b> 적용합니다.

" type="success" %}

{{site.data.alerts.important}}
픽셀이 <font color="#c7254e">상위 임곗값(threshold2)</font>보다 큰 기울기를 가지면 픽셀을 가장자리로 간주하고, <font color="#c7254e">하위 임곗값(threshold1)</font>보다 낮은 경우 가장자리로 고려하지 않습니다.
{{site.data.alerts.end}}

<blockquote class="formula">
<b>노름 계산식(Norm Formula):</b>
$$ L_1 = | \frac{dI}{dx} | + | \frac{dI}{dy} | $$
$$ L_2 = \sqrt{(\frac{dI}{dx})^2 + (\frac{dI}{dy})^2} $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지의 X와 Y에 대해 1차 미분을 계산한 다음, 네 방향으로 미분합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 캐니를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(edges)</a> 캐니가 적용된 이미지

> `하위 임곗값(threshold1)` 히스테리시스 하위 임곗값

> `상위 임곗값(threshold2)` 히스테리시스 상위 임곗값

> `마스크 크기(apertureSize)` 소벨 연산자의 마스크 크기

> `L2 그레이디언트(L2gradient)` L2 그레디이언트 사용 유/무

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(edges)</a> 캐니가 적용된 이미지