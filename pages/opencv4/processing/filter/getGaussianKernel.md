---
title: 가우시안 커널 반환
sidebar: opencv4_sidebar
permalink: getGaussianKernel
folder: opencv4
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">getGaussianKernel</h2>
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
<pre class="prettyprint"><code class="language-cpp">Mat cv::getGaussianKernel(
    int ksize,
    double sigma,
    int ktype = CV_64F
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-two">
<pre class="prettyprint"><code class="language-cs">Mat Cv2.GetGaussianKernel(
    int ksize,
    double sigma,
    MatType? ktype = null
)</code></pre>
            </div>
            <div class="tab-pane fade" id="service-three">
<pre class="prettyprint"><code class="language-py">retval = cv2.getGaussianKernel(
    ksize,
    sigma,
    ktype = None
)</code></pre>
            </div>
        </div>
    </div>
</div>

<br>

{{site.data.alerts.note}}
1차원 가우시안 커널을 생성합니다.<br>
<li class="alerts_li">더 높은 수준의 <a href="GaussianBlur">가우시안 흐림 효과(GaussianBlur)</a>을 활용할 수도 있습니다.</li>
{{site.data.alerts.end}}

{% include callout.html content="

- `커널 크기(ksize)`는 1 이상의 홀수여야 합니다.
  
- `시그마(sigma)`가 양수(Positive)가 아닌 경우 `시그마 계산식(Sigma Formula)`을 적용합니다.
  
- `필터 출력 정밀도(ktype)`는 `CV_32F` 형식, `CV_64F` 형식만 가능합니다.

" type="success" %}

<blockquote class="formula">
<b>시그마 계산식(Sigma Formula):</b>
$$ \sigma = 0.3 \times ( ( \frac {\text{ksize}-1}{2})-1)+0.8 $$
</blockquote>

<blockquote class="formula">
<b>가우시안 커널 계산식(Gaussian Kernel Formula):</b>
$$ G_i = \alpha \times e^{-\beta} $$
$$ \begin{matrix}
\alpha & \text{satisfied:} \sum_{i=0}^{\text{ksize}-1} G_{i} = 1
\end{matrix} $$
$$ \beta = \frac{(i-\frac{\text{ksize}-1}{2})^2}{ 2\sigma^2} $$
</blockquote>

<br>

### 요약(Summary)

> 1차원 가우시안 커널 필터 계수를 반환합니다.

### 매개변수(Parameter)

> `커널 크기(ksize)` 필터(커널)의 크기

> `시그마(sigma)` 가우스 커널 표준 편차

> `필터 출력 정밀도(ktype)` 필터 계수의 출력 정밀도 설정

### 반환값(Returns)

> `가우시안 필터 계수(retval)` 1차원 가우시안 커널 필터 계수
