---
title: 극좌표 변환
sidebar: opencv4_sidebar
permalink: warpPolar
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">warpPolar</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::warpPolar(
    Mat src,
    Mat dst,
    Mat dsize,
    Point2f center,
    double maxRadius,
    int flags
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.WarpPolar(
    Mat src,
    Mat dst,
    Size dsize,
    Point2f center,
    double maxRadius,
    InterpolationFlags interpolationFlags,
    WarpPolarMode warpPolarMode
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.warpPolar(
    src,
    dsize,
    center,
    maxRadius,
    flags
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>


{{site.data.alerts.note}}
<b>C++ OpenCV</b>와 <b>Python OpenCV</b>는 <font color="#c7254e">극좌표 플래그(flags)</font>에 <font color="#c7254e">내삽 방식(interpolation) + 극좌표 변환 방식(WarpPolarMode)</font>의 형태로 사용합니다.
{{site.data.alerts.end}}

{% include callout.html content="

`절대 크기(dsize)`의 **너비(Width)**와 **높이(Height)**가 0과 같거나 작은 경우
<br>
$$ \text{dsize.Area} = (maxRadius^2 \cdot \pi) $$
<br>
$$ \text{dsize.Width} = \text{round}(\text{maxRadius}) $$
<br>
$$ \text{dsize.Height} = \text{round}(\text{maxRadius}\cdot \pi) $$
<br><br>
`절대 크기(dsize)`의 **높이(Height)**가 0과 같거나 작은 경우
<br>
$$ \text{dsize.Height} = \text{round}(\text{dsize.Width}\cdot \pi) $$
<br>
" type="success" %}

{% include callout.html content="
`극좌표 변환 계산식(Polar Transform Formula)`
<br><br>
$$ dst(\rho, \phi) = src(x, y) $$
<br><br>
$$ \rho = \left\{\begin{matrix}
\frac{\text{dsize.Width}}{\text{maxRadius}} \cdot \text{magnitude}(\overrightarrow{I}) \\ 
\frac{\text{dsize.Width}}{log_e{\text{maxRadius}}} \cdot log_e{\text{magnitude}(\overrightarrow{I})} & \text{if} \ semilog
\end{matrix}\right. $$
<br><br>
$$ \phi = \frac{\text{dsize.Height}}{2\pi} \cdot angle(\overrightarrow{I}) $$
<br><br><br>
$$ \overrightarrow{I} = (x - \text{center}.x, \ y - \text{center}.y) $$
<br><br>
$$ magnitude(\overrightarrow{I}) = \sqrt{x(\overrightarrow{I})^2) + y(\overrightarrow{I})^2} $$
<br><br>
$$ angle(\overrightarrow{I}) = \text{atan2}(y(\overrightarrow{I}), \ x(\overrightarrow{I})) \cdot \frac{180}{\pi} $$
<br><br>
" type="success" %}

<br>

### 요약(Summary)

> 이미지에 극좌표 변환을 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 극좌표 변환을 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 극좌표 변환이 적용된 출력 이미지

> `절대 크기(dsize)` 출력 이미지의 크기

> `중심점(center)` 매핑 기준점

> `최대 반지름(maxRadius)` 변형하려는 크기(magnitude) 비율

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_Python}}">극좌표 플래그(flags)</a> 내삽 방식과 극좌표 변환 방식

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}" href="InterpolationFlags" style="cursor: revert;">내삽 방식(interpolation)</a> 이미지 내의 픽셀을 내삽하는데 사용되는 계산 방식

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C}}" href="WarpPolarMode" style="cursor: revert;">극좌표 변환 방식(warpPolarMode)</a> 극좌표 변환 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 극좌표 변환이 적용된 출력 이미지
