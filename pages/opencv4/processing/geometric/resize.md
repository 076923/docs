---
title: 크기 변환
sidebar: opencv4_sidebar
permalink: resize
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">resize</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::resize(
    Mat src,
    Mat dst,
    Size dsize,
    double fx = 0,
    double fy = 0,
    int interpolation = INTER_LINEAR
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.Resize(
    Mat src,
    Mat dst,
    Size dsize,
    double fx = 0,
    double fy = 0,
    InterpolationFlags interpolation = InterpolationFlags.Linear
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.resize(
    src,
    dsize,
    fx = None,
    fy = None,
    interpolation = None
)
</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
이미지를 <font color="#c7254e">확대</font>하는 경우에는 <b>픽셀에 대한 보간법</b>, <font color="#c7254e">이미지를 축소</font>하는 경우에는 <b>픽셀에 대한 병합법</b>이 수행됩니다.
{{site.data.alerts.end}}

{{site.data.alerts.tip}}
이미지에 <font color="#c7254e">상대 크기(fx, fy)</font>를 적용하려면 <font color="#c7254e">절대 크기(dsize)</font>에 (0, 0)을 할당해야 합니다.
<br>
<font color="#c7254e">절대 크기에 (0, 0)</font>을 할당하는 이유로는 <font color="#c7254e">상대 크기(fx, fy)</font>에서 계산된 크기가 <font color="#c7254e">절대 크기(dsize)</font>에 할당되어 크기를 변환하기 때문입니다.
{{site.data.alerts.end}}

<br>

{% include callout.html content="
`절대 크기(dsize)`
<br><br>
$$ \text{dsize.𝚠𝚒𝚍𝚝𝚑} = 𝚛𝚘𝚞𝚗𝚍(𝚏𝚡 \times \text{𝚜𝚛𝚌.𝚠𝚒𝚍𝚝𝚑}) $$
<br><br>
$$ \text{dsize.height} = 𝚛𝚘𝚞𝚗𝚍(𝚏𝚢 \times \text{𝚜𝚛𝚌.𝚑𝚎𝚒𝚐𝚑𝚝}) $$
<br><br>
`상대 크기(fx, fy)`
<br><br>
$$ fx = \frac{\text{dsize.𝚠𝚒𝚍𝚝𝚑}}{\text{src.𝚠𝚒𝚍𝚝𝚑}} $$
<br><br>
$$ fy = \frac{\text{dsize.height}}{\text{src.𝚑𝚎𝚒𝚐𝚑𝚝}} $$
" type="success" %}

<br>

### 요약(Summary)

> 이미지의 크기를 변환합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 크기를 변경하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 크기가 변경된 출력 이미지

> `절대 크기(dsize)` 크기를 변경하려는 이미지의 너비, 높이 값

> `상대 크기 X(fx)` 크기를 변경하려는 이미지의 너비 비율

> `상대 크기 Y(fy)` 크기를 변경하려는 이미지 높이 비율

> [`내삽 방식(interpolation)`](InterpolationFlags) 이미지 내의 픽셀을 내삽하는데 사용되는 계산 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 크기가 변경된 출력 이미지
