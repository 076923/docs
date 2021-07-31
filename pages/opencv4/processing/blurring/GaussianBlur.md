---
title: 가우시안 흐림 효과
sidebar: opencv4_sidebar
permalink: GaussianBlur
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">GaussianBlur</h2>
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
<pre class="prettyprint"><code class="language-cpp">void cv::GaussianBlur(
    Mat src,
    Mat dst,
    Size ksize,
    double sigmaX,
    double sigmaY = 0,
    int borderType = BORDER_DEFAULT
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">void Cv2.GaussianBlur(
    Mat src,
    Mat dst,
    Size ksize,
    double sigmaX,
    double sigmaY = 0,
    BorderTypes borderType = BorderTypes.Reflect101
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">dst = cv2.GaussianBlur(
    src,
    ksize,
    sigmaX,
    sigmaY = None,
    borderType = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
가우시안 커널을 사용하여 이미지를 흐리게합니다.
{{site.data.alerts.end}}

{% include callout.html content="

- `입력 이미지(src)`는 `CV_8U` 형식, `CV_16U` 형식, `CV_16S` 형식, `CV_32F` 형식, `CV_64F` 형식을 할당할 수 있습니다.
  
- `출력 이미지(dst)`는 `입력 이미지(src)`와 동일한 정밀도를 반환합니다.
  
" type="success" %}

{% include callout.html content="

- `커널 크기(ksize)`의 너비와 높이는 0 이상이며, 홀수여야 합니다.
  
- `시그마Y(sigmaY)`가 0인 경우 `시그마Y(sigmaY)`의 값은 `시그마X(sigmaX)`의 값과 같아집니다.
  
- `시그마X(sigmaX)`와 `시그마Y(sigmaY)`의 값을 모두 0으로 설정한다면 `커널 크기(ksize)`에 의해 자동으로 설정됩니다.

" type="success" %}

<blockquote class="formula">
<b>시그마 계산식(Sigma Formula):</b>
$$ \sigma_x = 0.3 \times ( ( \frac {\text{ksize.width}-1}{2})-1)+0.8 $$
$$ \sigma_y = 0.3 \times ( ( \frac {\text{ksize.height}-1}{2})-1)+0.8 $$
</blockquote>

<br>

### 요약(Summary)

> 입력 이미지에 가우스 필터를 이미지에 적용합니다.

### 매개변수(Parameter)

> `입력 이미지(src)` 가우시안 흐림 효과를 적용하려는 입력 이미지

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_C_CS}}">출력 이미지(dst)</a> 가우시안 흐림 효과가 적용된 이미지

> `커널 크기(ksize)` 커널의 크기(너비, 높이)

> `시그마 X(sigmaX)` X 방향의 가우스 커널 표준 편차

> `시그마 Y(sigmaY)` Y 방향의 가우스 커널 표준 편차

> `오프셋(delta)` 필터링 된 픽셀에 더해지는 값

> [`외삽 방식(borderType)`](BorderTypes) 이미지 밖의 픽셀을 외삽하는데 사용되는 방식

### 반환값(Returns)

> <a data-toggle="tooltip" data-original-title="{{site.data.glossary.only_Python}}">출력 이미지(dst)</a> 가우시안 흐림 효과가 적용된 이미지